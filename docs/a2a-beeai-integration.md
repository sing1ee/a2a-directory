# A2A Protocol integration in BeeAI Framework (Python）

The BeeAI Framework is an open-source framework for building production-grade multi-agent systems. Hosted by the Linux Foundation under open governance, it ensures transparency, community-driven development, and enterprise-grade stability. The framework provides seamless integration with multiple protocols, including Agent-to-Agent (A2A) protocol and Model Context Protocol (MCP).

The A2A protocol enables direct communication between autonomous agents, allowing them to collaborate, share context, and distribute tasks across different systems and networks.

## Prerequisites 

- Python 3.8+
- BeeAI Framework installed with A2A support: `pip install "beeai-framework[a2a]"`
- Ollama or an LLM API key (e.g., Gemini, OpenAI, etc.)

## Table of Contents

- [Server Implementation](#server-implementation)
    - [Basic Server Example](#basic-server-example)
    - [Advanced Server Configuration](#advanced-server-configuration) 
- [Client Implementation](#client-implementation)
    - [Basic Client Example](#basic-client-example)

## Server Implementation

### Basic Server Example

The simplest A2A server setup requires just four lines of code:

```python
from beeai_framework.adapters.a2a import A2AServer
from beeai_framework.agents.experimental import RequirementAgent
from beeai_framework.backend.models.gemini import GeminiChatModel

# 1. Define the LLM
llm = GeminiChatModel(api_key="your_api_key_here")

# 2. Create the agent
agent = RequirementAgent(llm=llm)

# 3. Register the agent with the A2A server
server = A2AServer().register(agent)

# 4. Start the server
server.serve()
```

This creates a basic A2A server running on `localhost:9999` with default settings.

### Advanced Server Configuration

If you want to customize the agent or configure the A2A server, you can use optional parameters. You can configure many aspects such as the host, port, provide your own MemoryManager implementation for managing a stateful server, or provide the agent's metadata.

Here's an example using a RequirementAgent with tools and unlimited memory, running on port 9999, with context memory for 100 clients:

```python
from beeai_framework.adapters.a2a import A2AServer, A2AServerConfig
from beeai_framework.agents.experimental import RequirementAgent
from beeai_framework.backend import ChatModel
from beeai_framework.memory import UnconstrainedMemory
from beeai_framework.serve.utils import LRUMemoryManager
from beeai_framework.tools.search.duckduckgo import DuckDuckGoSearchTool
from beeai_framework.tools.weather import OpenMeteoTool


def main() -> None:
    # Initialize the language model
    llm = ChatModel.from_name("gemini:gemini-2.5-flash")

    # Create agent with tools and memory
    agent = RequirementAgent(
        llm=llm,
        tools=[DuckDuckGoSearchTool(), OpenMeteoTool()],
        memory=UnconstrainedMemory(),
    )

    # Configure and start the A2A server
    A2AServer(
        config=A2AServerConfig(host="0.0.0.0", port=9999),
        memory_manager=LRUMemoryManager(maxsize=100)
    ).register(
        agent,
        description="Simple Chat agent",
        version="1.0"
    ).serve()


if __name__ == "__main__":
    main()
```

## Client Implementation

Consuming a remote agent is even simpler than exposing one. You just need to provide its URL and memory configuration.

### Basic Client Example

```python
import asyncio
import sys
import traceback

from beeai_framework.adapters.a2a.agents import A2AAgent
from beeai_framework.errors import FrameworkError
from beeai_framework.memory.unconstrained_memory import UnconstrainedMemory
from examples.helpers.io import ConsoleReader


async def main() -> None:
    reader = ConsoleReader()

    # Create A2A client agent
    agent = A2AAgent(
        url="http://127.0.0.1:9999",
        memory=UnconstrainedMemory()
    )
    for prompt in reader:
        # Run the agent and observe events
        response = await agent.run(prompt).on(
            "update",
            lambda data, event: (reader.write("Agent 🤖 (debug) : ", data)),
        )

        reader.write("Agent 🤖 : ", response.result.text)


if __name__ == "__main__":
    try:
        asyncio.run(main())
    except FrameworkError as e:
        traceback.print_exc()
        sys.exit(e.explain())
```

---

Check out the [BeeAI Framework Documentation](https://framework.beeai.dev/introduction/welcome) to learn more!
