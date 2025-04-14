# Python A2A: A Comprehensive Guide to Google's Agent-to-Agent Protocol

## Introduction

Python A2A is an implementation of Google's Agent-to-Agent (A2A) protocol, designed to standardize communication between AI agents. This protocol solves a major challenge in the AI ecosystem: enabling different AI services to communicate seamlessly without custom translation layers.

As the AI landscape fragments into specialized services, each with its own API format and parameters, developers spend excessive time building communication infrastructure rather than focusing on AI logic. Python A2A addresses this by providing a standardized way for AI agents to talk to each other, regardless of their underlying implementation.

## Getting Started with Python A2A

### Installation

```bash
# Basic installation
pip install python-a2a

# For OpenAI integration
pip install "python-a2a[openai]"

# For Anthropic Claude integration
pip install "python-a2a[anthropic]"

# For all optional dependencies
pip install "python-a2a[all]"
```

## Core Concepts

Python A2A implements several key concepts from the A2A protocol:

1. **Message Structure**: Defined formats for text, function calls, and responses
2. **Conversation Threading**: Support for maintaining context across interactions
3. **Function Calling**: Standardized way for agents to expose and call functions
4. **Error Handling**: Consistent error formats

## Building Your First A2A Agent

Let's start with a simple echo agent that responds to messages:

```python
from python_a2a import A2AServer, Message, TextContent, MessageRole, run_server

class EchoAgent(A2AServer):
    """A simple agent that echoes back messages with a prefix."""
    
    def handle_message(self, message):
        if message.content.type == "text":
            return Message(
                content=TextContent(text=f"Echo: {message.content.text}"),
                role=MessageRole.AGENT,
                parent_message_id=message.message_id,
                conversation_id=message.conversation_id
            )

# Run the server
if __name__ == "__main__":
    agent = EchoAgent()
    run_server(agent, host="0.0.0.0", port=5000)
```

Now, let's create a client to talk to our agent:

```python
from python_a2a import A2AClient, Message, TextContent, MessageRole

# Create a client to talk to our agent
client = A2AClient("http://localhost:5000/a2a")

# Send a message
message = Message(
    content=TextContent(text="Hello, is this thing on?"),
    role=MessageRole.USER
)
response = client.send_message(message)

# Print the response
print(f"Agent says: {response.content.text}")
```

## Function Calling Between Agents

One of the powerful features of A2A is standardized function calling. Here's a calculator agent that exposes mathematical functions:

```python
import math
from python_a2a import (
    A2AServer, Message, TextContent, FunctionCallContent, 
    FunctionResponseContent, FunctionParameter, MessageRole, run_server
)

class CalculatorAgent(A2AServer):
    """An agent that provides mathematical calculation functions."""
    
    def handle_message(self, message):
        if message.content.type == "text":
            return Message(
                content=TextContent(
                    text="I'm a calculator agent. You can call my functions:\n"
                         "- calculate: Basic arithmetic (operation, a, b)\n"
                         "- sqrt: Square root (value)"
                ),
                role=MessageRole.AGENT,
                parent_message_id=message.message_id,
                conversation_id=message.conversation_id
            )
            
        elif message.content.type == "function_call":
            function_name = message.content.name
            params = {p.name: p.value for p in message.content.parameters}
            
            try:
                if function_name == "calculate":
                    operation = params.get("operation", "add")
                    a = float(params.get("a", 0))
                    b = float(params.get("b", 0))
                    
                    if operation == "add":
                        result = a + b
                    elif operation == "subtract":
                        result = a - b
                    elif operation == "multiply":
                        result = a * b
                    elif operation == "divide":
                        if b == 0:
                            raise ValueError("Cannot divide by zero")
                        result = a / b
                    else:
                        raise ValueError(f"Unknown operation: {operation}")
                    
                    return Message(
                        content=FunctionResponseContent(
                            name="calculate",
                            response={"result": result}
                        ),
                        role=MessageRole.AGENT,
                        parent_message_id=message.message_id,
                        conversation_id=message.conversation_id
                    )
                
                elif function_name == "sqrt":
                    value = float(params.get("value", 0))
                    if value < 0:
                        raise ValueError("Cannot calculate square root of negative number")
                    
                    result = math.sqrt(value)
                    return Message(
                        content=FunctionResponseContent(
                            name="sqrt",
                            response={"result": result}
                        ),
                        role=MessageRole.AGENT,
                        parent_message_id=message.message_id,
                        conversation_id=message.conversation_id
                    )
                    
            except Exception as e:
                return Message(
                    content=FunctionResponseContent(
                        name=function_name,
                        response={"error": str(e)}
                    ),
                    role=MessageRole.AGENT,
                    parent_message_id=message.message_id,
                    conversation_id=message.conversation_id
                )

if __name__ == "__main__":
    agent = CalculatorAgent()
    run_server(agent, host="0.0.0.0", port=5001)
```

Here's how to call the calculator agent's functions:

```python
from python_a2a import (
    A2AClient, Message, FunctionCallContent, 
    FunctionParameter, MessageRole
)

client = A2AClient("http://localhost:5001/a2a")

# Create a function call message
function_call = Message(
    content=FunctionCallContent(
        name="calculate",
        parameters=[
            FunctionParameter(name="operation", value="add"),
            FunctionParameter(name="a", value=5),
            FunctionParameter(name="b", value=3)
        ]
    ),
    role=MessageRole.USER
)

response = client.send_message(function_call)

if response.content.type == "function_response":
    result = response.content.response.get("result")
    if result is not None:
        print(f"Result: {result}")  # Output: Result: 8
```

## LLM-Powered Agents

Python A2A includes ready-to-use integrations with popular LLM providers. Here's an OpenAI-powered agent:

```python
import os
from python_a2a import OpenAIA2AServer, run_server

# Create an agent powered by OpenAI
agent = OpenAIA2AServer(
    api_key=os.environ["OPENAI_API_KEY"],
    model="gpt-4",
    system_prompt="You are a helpful AI assistant."
)

# Run the server
if __name__ == "__main__":
    run_server(agent, host="0.0.0.0", port=5002)
```

Similarly, you can create an Anthropic Claude-powered agent:

```python
import os
from python_a2a import ClaudeA2AServer, run_server

# Create an agent powered by Anthropic Claude
agent = ClaudeA2AServer(
    api_key=os.environ["ANTHROPIC_API_KEY"],
    model="claude-3-opus-20240229",
    system_prompt="You are a helpful AI assistant."
)

# Run the server
if __name__ == "__main__":
    run_server(agent, host="0.0.0.0", port=5003)
```

## Multi-Agent Workflows

The real power of A2A comes when you connect multiple agents. Let's build a research assistant workflow:

```python
from python_a2a import (
    A2AClient, Message, TextContent, MessageRole, Conversation
)

def research_workflow(query):
    # Connect to the specialized agents
    llm_client = A2AClient("http://localhost:5002/a2a")     # LLM agent
    search_client = A2AClient("http://localhost:5003/a2a")  # Search agent
    summarize_client = A2AClient("http://localhost:5004/a2a")  # Summarize agent
    
    # Track the entire workflow in a conversation
    conversation = Conversation()
    conversation.create_text_message(
        text=f"Research question: {query}",
        role=MessageRole.USER
    )
    
    # Step 1: Generate search queries
    print("Generating search queries...")
    search_request = Message(
        content=TextContent(
            text=f"Based on this research question: '{query}', "
                 f"generate 3 specific search queries that would help find relevant information."
        ),
        role=MessageRole.USER
    )
    search_queries_response = llm_client.send_message(search_request)
    conversation.add_message(search_queries_response)
    
    # Step 2: Retrieve information
    print("Retrieving information...")
    search_message = Message(
        content=TextContent(
            text=f"Search for information to answer: {query}\n\n"
                 f"Using these queries:\n{search_queries_response.content.text}"
        ),
        role=MessageRole.USER
    )
    search_results = search_client.send_message(search_message)
    conversation.add_message(search_results)
    
    # Step 3: Synthesize information
    print("Synthesizing information...")
    summarize_message = Message(
        content=TextContent(
            text=f"Synthesize this information to answer the question: '{query}'\n\n"
                 f"Information:\n{search_results.content.text}"
        ),
        role=MessageRole.USER
    )
    summary_response = summarize_client.send_message(summarize_message)
    conversation.add_message(summary_response)
    
    # Add final answer to the conversation
    conversation.create_text_message(
        text=f"Answer to your research question:\n\n{summary_response.content.text}",
        role=MessageRole.AGENT
    )
    
    return conversation

# Example usage
if __name__ == "__main__":
    query = input("What's your research question? ")
    result = research_workflow(query)
    print("\nResearch Complete!")
    print("=" * 50)
    print(result.messages[-1].content.text)
```

## Advanced Example: Weather and Trip Planning with A2A

Here's an example demonstrating how A2A simplifies communication between agents:

```python
from python_a2a import A2AClient, Message, TextContent, MessageRole

# With A2A: Any agent -> Any other agent
def plan_trip(location):
    # Connect to specialized agents - all using the same protocol
    weather_client = A2AClient("http://localhost:5001/a2a")
    openai_client = A2AClient("http://localhost:5002/a2a")
    
    # Ask weather agent
    weather_message = Message(
        content=TextContent(text=f"What's the weather forecast for {location}?"),
        role=MessageRole.USER
    )
    weather_response = weather_client.send_message(weather_message)
    
    # Ask OpenAI agent, including weather info
    planning_message = Message(
        content=TextContent(
            text=f"I'm planning a trip to {location}. Weather forecast: {weather_response.content.text}"
                 f"Please suggest activities."
        ),
        role=MessageRole.USER
    )
    planning_response = openai_client.send_message(planning_message)
    
    return planning_response.content.text

# This works with ANY A2A-compatible agents - no custom adapters needed!
```

## Managing Conversations

Python A2A provides a `Conversation` class to manage multi-turn interactions:

```python
from python_a2a import Conversation, MessageRole, A2AClient

# Create a new conversation
conversation = Conversation()

# Add a user message
conversation.create_text_message(
    text="What's the weather like today?",
    role=MessageRole.USER
)

# Connect to an agent
weather_agent = A2AClient("http://localhost:5001/a2a")

# Send the last message in the conversation
last_message = conversation.messages[-1]
response = weather_agent.send_message(last_message)

# Add the response to the conversation
conversation.add_message(response)

# Continue the conversation
conversation.create_text_message(
    text="Thanks! Will I need an umbrella?",
    role=MessageRole.USER
)

# Send the new message, including conversation history
response = weather_agent.send_message(
    conversation.messages[-1],
    conversation_id=conversation.conversation_id
)

# Add this response too
conversation.add_message(response)

# Print the entire conversation
for msg in conversation.messages:
    role = "User" if msg.role == MessageRole.USER else "Agent"
    print(f"{role}: {msg.content.text}")
```

## Error Handling

Python A2A provides standardized error handling:

```python
from python_a2a import A2AClient, Message, TextContent, MessageRole

client = A2AClient("http://localhost:5001/a2a")

try:
    message = Message(
        content=TextContent(text="Hello"),
        role=MessageRole.USER
    )
    response = client.send_message(message)
    
except ConnectionError as e:
    print(f"Connection error: {e}")
    
except TimeoutError as e:
    print(f"Timeout error: {e}")
    
except Exception as e:
    print(f"Unexpected error: {e}")
```

## Creating Custom A2A Agents

Here's a template for creating your own A2A-compatible agent:

```python
from python_a2a import A2AServer, Message, TextContent, MessageRole, run_server

class MyCustomAgent(A2AServer):
    def __init__(self, **kwargs):
        super().__init__(**kwargs)
        # Initialize your agent-specific components here
    
    def handle_message(self, message):
        """Process incoming messages and return responses.
        
        This is the main entry point for handling messages in your agent.
        """
        if message.content.type == "text":
            # Process text messages
            user_text = message.content.text
            
            # Generate your response (replace with your logic)
            response_text = f"You said: {user_text}"
            
            return Message(
                content=TextContent(text=response_text),
                role=MessageRole.AGENT,
                parent_message_id=message.message_id,
                conversation_id=message.conversation_id
            )
            
        elif message.content.type == "function_call":
            # Handle function calls (if your agent supports them)
            # ...
            pass
            
        # Return a default response if no other conditions matched
        return Message(
            content=TextContent(text="I don't know how to handle this message type."),
            role=MessageRole.AGENT,
            parent_message_id=message.message_id,
            conversation_id=message.conversation_id
        )

# Run your agent
if __name__ == "__main__":
    my_agent = MyCustomAgent()
    run_server(my_agent, host="0.0.0.0", port=5005)
```

## Conclusion

Python A2A provides a standardized way for AI agents to communicate, making it easier to build multi-agent systems. By adopting this protocol, you can:

1. Reduce development time spent on communication infrastructure
2. Easily swap and upgrade agent implementations
3. Build modular, extensible AI systems
4. Leverage specialized agents for different tasks

The A2A protocol and its Python implementation are helping to build a future where AI systems can be composed like LEGO blocks, with specialized agents working together seamlessly.

For more information, check out the Python A2A GitHub repository, PyPI page, and documentation.