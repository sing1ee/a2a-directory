# A2A Protocol integration in BeeAI Framework （Python）

## Overview

BeeAI Framework is an open-source framework for building production-grade multi-agent systems. It is hosted by the Linux Foundation under open governance, ensuring transparency, community-driven development, and enterprise-grade stability. BeeAI Framework provides a simple way to integrate with multiple protocols like MCP and a2a.

## Table of Contents

1. [Server Implementation](#server-implementation)
2. [Client Implementation](#client-implementation)

## Server Implementation

Exposing an agent with MCP is as simple as it can be using the BeeaI Framework. For a default exposure, four steps are sufficient:

1. defining the LLM

```python
    llm = GeminiChatModel(api_key="xxx")
```

2. creating the agent

```python
    agent = RequirementAgent(llm=llm)
```

3. registering the agent with the a2a server

```python
    server = A2AServer().register(agent)
```

4. starting the server.

```python
    server.serve()
```

If you want to further customize the agent or configure the a2a server itself, it's possible using optional parameters. You can configure many parameters, such as the host, port, provide your own MemoryManager implementation for managing a stateful server, or provide the agent's metadata itself.

In the example below, we'll use a RequirementAgent with two tools and unlimited memory. We'll register it with the a2a server and run it on port 9999. We'll allow it to remember the context for 100 clients and define its description and version.

```python
from beeai_framework.adapters.a2a import A2AServer, A2AServerConfig
from beeai_framework.agents.experimental import RequirementAgent
from beeai_framework.backend import ChatModel
from beeai_framework.memory import UnconstrainedMemory
from beeai_framework.serve.utils import LRUMemoryManager
from beeai_framework.tools.search.duckduckgo import DuckDuckGoSearchTool
from beeai_framework.tools.weather import OpenMeteoTool


def main() -> None:
    llm = ChatModel.from_name("gemini:gemini-2.5-flash")
    agent = RequirementAgent(
        llm=llm,
        tools=[DuckDuckGoSearchTool(), OpenMeteoTool()],
        memory=UnconstrainedMemory(),
    )

    A2AServer(
        config=A2AServerConfig(port=9999), memory_manager=LRUMemoryManager(maxsize=100)
    ).register(agent, description="Simple Chat agent", version="1.0").serve()


if __name__ == "__main__":
    main()
```

## Client Implementation

Consuming a remote agent is even simpler than exposing one. You just need to provide its URL and a Memory.

In the following example is a demonstration of a simple chat interface for an a2a agent running on localhost on port 9999.

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

    agent = A2AAgent(url="http://127.0.0.1:9999", memory=UnconstrainedMemory())
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
