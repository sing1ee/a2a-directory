# ✨ Agent2Agent Protocol ✨

![Awesome A2A](/images/a2a-protocol.png)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md)

<a id="contents"></a>
## Contents

- 📋 [Overview](#overview)
- 🚀 [Getting Started](#getting-started)
- 📚 [Resources](#resources)
- 💻 [Implementations](#implementations)
- 🎴 [AgentCard](#agentcard)
- 🤝 [Community Implementations](#community-implementations)
- 👥 [Community](#community)
- 🤝 [Contributing](#contributing)


## Overview

A2A (Agent2Agent) is an open protocol from Google enabling AI agents to communicate securely and collaborate. It breaks down silos between isolated agent systems, allowing for complex cross-application automation.

**Key Features:**
- 🎯 Simple: Uses HTTP, JSON-RPC, SSE
- 🏢 Enterprise Ready: Focuses on security and privacy
- ⚡ Async First: Handles long-running tasks
- 🔄 Modality Agnostic: Supports text, files, forms, streams
- 🔒 Opaque Execution: Agents interact without sharing internal logic

**Official Links:**
- 🌐 Website: [google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub: [github.com/google/A2A](https://github.com/google/A2A)

## Getting Started

1. **Learn the Basics**
   - 📖 Read the [technical documentation](https://google.github.io/A2A/#/documentation)
   - 🎥 Watch the [demo video](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **Run Samples**
   - 📥 Clone the [official repo](https://github.com/google/A2A)
   - 📝 Follow instructions in `/samples`

3. **Build Your Own**
   - 🛠️ Use official libraries or adapt samples
   - 🏗️ Start with a basic A2A agent or client


## Resources

### Official Documentation
- 🇺🇸 [Technical Documentation](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON Specification](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [Agent Card Specification](https://google.github.io/A2A/#/documentation?id=agent-card)

### Community Documentation
- 🇺🇸 [A2A TypeScript Guide](docs/a2a-typescript-guide.md) - A comprehensive guide for implementing A2A in TypeScript
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - Comparison between A2A and Model Context Protocol
- 🇺🇸 [Understanding A2A Protocol](docs/understanding-a2a-protocol.md) - Deep dive into A2A protocol concepts
- 🇺🇸 [A2A Sample Methods and JSON Responses](docs/a2a-sample-methods-and-json-responses.md) - Detailed examples of A2A methods and responses
- 🇺🇸 [Python A2A](docs/python-a2a.md): A powerful and easy-to-use library for implementing Google's [Agent-to-Agent (A2A) protocol](https://google.github.io/A2A/) - [Link](https://a2aprotocol.ai/blog/python-a2a)
- 🇨🇳 [A2A 协议介绍](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A 协议的中文介绍

[⬆️ Back to Contents](#contents)

## Implementations

### Official Samples

#### Python
- 🐍 **Common Library**: Core HTTP, JSON-RPC, SSE handling - [Link](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **Host (Client)**: Command-line client example - [Link](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **Host (Agent)**: Orchestrator agent delegating to A2A agents - [Link](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **Server Library**: Core server implementation - [Link](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **Client Library**: Client implementation - [Link](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **Host (Client)**: Command-line client example - [Link](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

## Community Implementations

| Name | Author | Description | Stars |
|------|--------|-------------|-------|
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | A TypeScript implementation of the A2A protocol with a focus on modularity and extensibility | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | A Go library for building A2A servers, with example implementations | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | An idiomatic Rust implementation following hexagonal architecture principles | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | A minimalistic Python SDK for A2A communication | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A C#/.NET implementation of the A2A protocol | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | A module for integrating the A2A protocol into NestJS applications | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | An easy-to-use Python library for implementing the A2A protocol | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | An A2A network implementation for hosting, registering, discovering, and interacting with agents | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | An AI agent development framework built on Google's ADK, facilitating agent creation potentially for A2A networks | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |

[⬆️ Back to Contents](#contents)

### Framework Integrations

#### Python
- 🐍 **LangGraph**: Currency conversion (Features: Tools, Streaming, Multi-turn) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**: Image generation (Features: Non-textual Artifacts (Files)) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**: Expense reimbursement (Features: Multi-turn, Forms (DataPart)) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**: A powerful and easy-to-use library for implementing Google's [Agent-to-Agent (A2A) protocol](https://google.github.io/A2A/) - [Link](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**: Movie info / Code generation (Features: Tools, Artifacts (Files), Async) - [Link](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### Community Samples

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**: A Coder Agent implementation with A2A Server and Client - [Link](https://github.com/sing1ee/a2a-agent-coder)

[⬆️ Back to Contents](#contents)

## AgentCard

## Community

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first. 