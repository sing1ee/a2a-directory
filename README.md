# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## Contents

- 📋 [Overview](#overview)
- 🚀 [Getting Started](#getting-started)
- 📚 [Resources](#resources)
- 📦 [Official Samples](#official-samples)
- 🛠️ [Tools](#tools)
- 🤝 [Community Implementations](#community-implementations)
- 🎯 [Community Samples](#community-samples)
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
- 📦 GitHub: [https://github.com/google-a2a/A2A](https://github.com/google-a2a/A2A)

## Getting Started

1. **Learn the Basics**
   - 📖 Read the [technical documentation](https://google.github.io/A2A/#/documentation)
   - 🎥 Watch the [demo video](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **Run Samples**
   - 📥 Clone the [official repo](https://github.com/google-a2a/a2a-samples)
   - 📝 Follow instructions in `/samples`

3. **Build Your Own**
   - 🛠️ Use official libraries or adapt samples
   - 🏗️ Start with a basic A2A agent or client


## Resources

### Official Documentation
- 🇺🇸 [Technical Documentation](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON Specification](https://github.com/google-a2a/A2A/tree/main/specification)
- 🇺🇸 [Agent Card Specification](https://google-a2a.github.io/A2A/specification/#5-agent-discovery-the-agent-card)

## Official Samples

### Python Sample Collection

#### Agent Examples (Intelligent Agents Based on Different Frameworks)

| Project Name | Description | Link |
|-------------|-------------|------|
| Google ADK | Expense report filling agent, showcasing multi-turn interactions and web form handling | [google_adk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/google_adk) |
| AG2 + MCP | MCP-enabled agent based on AG2 framework | [ag2](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/ag2) |
| Azure AI Foundry | Agent based on Azure AI Foundry services | [azureaifoundry_sdk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/azureaifoundry_sdk) |
| LangGraph | Currency conversion agent with tool usage and streaming updates | [langgraph](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/langgraph) |
| CrewAI | Image generation agent with multi-turn interactions and image transmission | [crewai](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/crewai) |
| LlamaIndex | File parsing and chat agent with file upload and streaming updates | [llama_index_file_chat](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/llama_index_file_chat) |
| Marvin | Contact information extraction agent | [marvin](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/marvin) |
| MindsDB | Enterprise data agent supporting database queries | [mindsdb](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/mindsdb) |
| Semantic Kernel | Travel agent based on Microsoft Semantic Kernel framework | [semantickernel](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/semantickernel) |
| AutoGen | AutoGen framework example | [autogen](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/autogen) |
| Hello World | Basic example agent | [helloworld](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/helloworld) |
| Veo Video Generation | Video generation agent | [veo_video_gen](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/veo_video_gen) |
| Analytics | Analytics agent | [analytics](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/analytics) |
| A2A Telemetry | Telemetry data agent | [a2a_telemetry](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/a2a_telemetry) |
| A2A MCP | MCP protocol agent | [a2a_mcp](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/a2a_mcp) |
| Birthday Planner ADK | Birthday planning agent | [birthday_planner_adk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/birthday_planner_adk) |
| Headless Agent Auth | Headless agent authentication example | [headless_agent_auth](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/headless_agent_auth) |

#### Host Applications (Client Applications)

| Project Name | Description | Link |
|-------------|-------------|------|
| CLI | Command line client | [cli](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/hosts/cli) |
| Multiagent | Multi-agent orchestrator | [multiagent](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/hosts/multiagent) |

### Go Language Examples

| Project Name | Description | Link |
|-------------|-------------|------|
| Server | Go language A2A server implementation | [server](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/server) |
| Client | Go language A2A client implementation | [client](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/client) |
| Models | Shared data structures | [models](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/models) |

### JavaScript/TypeScript Examples

| Project Name | Description | Link |
|-------------|-------------|------|
| Movie Agent | Movie information search agent using TMDB API | [movie-agent](https://github.com/google-a2a/a2a-samples/tree/main/samples/js/src/agents/movie-agent) |
| Coder Agent | Code generation agent | [coder](https://github.com/google-a2a/a2a-samples/tree/main/samples/js/src/agents/coder) |



## Tools

Essential tools for A2A protocol development, testing, and validation.

**🔗 [A2A Protocol Validator](https://a2aprotocol.ai/a2a-protocol-validator)**


[⬆️ Back to Contents](#contents)


## Community Implementations

| Name | Author | Description | Stars |
|------|--------|-------------|-------|
| [a2a-python](https://github.com/google/a2a-python) | [@google](https://github.com/google) | Official Python SDK for the Agent2Agent (A2A) Protocol | [![Stars](https://img.shields.io/github/stars/google/a2a-python?style=social)](https://github.com/google/a2a-python) |
| [a2a-js](https://github.com/google-a2a/a2a-js) | [@google-a2a](https://github.com/google-a2a) | Official JavaScript SDK for the Agent2Agent (A2A) Protocol - A JavaScript library that helps run agentic applications as A2AServers | [![Stars](https://img.shields.io/github/stars/google-a2a/a2a-js?style=social)](https://github.com/google-a2a/a2a-js) |
| [a2a-java](https://github.com/a2aproject/a2a-java) | [@a2aproject](https://github.com/a2aproject) | Official Java SDK for the Agent2Agent (A2A) Protocol - A Java library that helps run agentic applications as A2AServers | [![Stars](https://img.shields.io/github/stars/a2aproject/a2a-java?style=social)](https://github.com/a2aproject/a2a-java) |
| [a2a-go](https://github.com/a2aproject/a2a-go) | [@a2aproject](https://github.com/a2aproject) | Official Go SDK for the Agent2Agent (A2A) Protocol | [![Stars](https://img.shields.io/github/stars/a2aproject/a2a-go?style=social)](https://github.com/a2aproject/a2a-go) |
| [a2ajava](https://github.com/vishalmysore/a2ajava) | [@vishalmysore](https://github.com/vishalmysore) | A pure Java implementation of Google's A2A protocol for Spring Boot applications, featuring both client and server implementations | [![Stars](https://img.shields.io/github/stars/vishalmysore/a2ajava?style=social)](https://github.com/vishalmysore/a2ajava) |
| [a2a4j](https://github.com/a2ap/a2a4j) | [@a2ap](https://github.com/a2ap) | A2A4J is a comprehensive Java implementation of the Agent2Agent Protocol, including server, client, examples, and a starter — ready to use out of the box. | [![Stars](https://img.shields.io/github/stars/a2ap/a2a4j?style=social)](https://github.com/a2ap/a2a4j) |
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | A TypeScript implementation of the A2A protocol with a focus on modularity and extensibility | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [trpc-a2a-go](https://github.com/trpc-group/trpc-a2a-go) | [@trpc-group](https://github.com/trpc-group) | Go A2A implementation by the tRPC team featuring full client/server support, in-memory task management, streaming responses, session management, multiple auth methods (JWT, API Key, OAuth2), and comprehensive examples | [![Stars](https://img.shields.io/github/stars/trpc-group/trpc-a2a-go?style=social)](https://github.com/trpc-group/trpc-a2a-go) |
| [jira-a2a](https://github.com/tuannvm/jira-a2a) | [@tuannvm](https://github.com/tuannvm) | The Jira A2A system is a DevOps workflow automation platform using the tRPC-A2A-Go framework. It consists of independent Go agents that communicate via A2A messages. | [![Stars](https://img.shields.io/github/stars/tuannvm/jira-a2a?style=social)](https://github.com/tuannvm/jira-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | A Go library for building A2A servers, with example implementations | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | An idiomatic Rust implementation following hexagonal architecture principles | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | A minimalistic Python SDK for A2A communication | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A C#/.NET implementation of the A2A protocol | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | A module for integrating the A2A protocol into NestJS applications | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | An easy-to-use Python library for implementing the A2A protocol | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | An A2A network implementation for hosting, registering, discovering, and interacting with agents | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | An AI agent development framework built on Google's ADK, facilitating agent creation potentially for A2A networks | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | A lightweight A2A python implementation | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A command-line client for the A2A | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A Test Suit](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A Test Suite | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | A Self-hosted Browser Using Agent with built-in MCP and A2A support | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | A multi-agent chat application with MCP support, aiming to expose agents via the A2A protocol and connect to remote A2A agents as a client | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | A JS/TS SDK for the Agent2Agent Protocol with a focus on developer experience and comprehensive features | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |
| [a2a-validation-tool](https://github.com/llmx-de/a2a-validation-tool) | [@llmx-de](https://github.com/llmx-de) | A desktop application for testing and validating Agent-to-Agent (A2A) protocol implementations | [![Stars](https://img.shields.io/github/stars/llmx-de/a2a-validation-tool?style=social)](https://github.com/llmx-de/a2a-validation-tool) |
| [Protolink](https://github.com/nMaroulis/protolink) | [@nMaroulis](https://github.com/nMaroulis) | A Python library for building autonomous Agents with Agent-to-Agent (A2A) protocol implementations, integrating LLMs and tools. | [![Stars](https://img.shields.io/github/stars/nMaroulis/protolink?style=social)](https://github.com/nMaroulis/protolink) |

[⬆️ Back to Contents](#contents)


### Community Samples

| Name | Author | Description | Stars |
|------|--------|-------------|-------|
| [a2a-agent-coder](https://github.com/sing1ee/a2a-agent-coder) | [@sing1ee](https://github.com/sing1ee) | A Coder Agent implementation with A2A Server and Client | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-agent-coder?style=social)](https://github.com/sing1ee/a2a-agent-coder) |
| [agentic-trading](https://github.com/kweinmeister/agentic-trading) | [@kweinmeister](https://github.com/kweinmeister) | A sample application demonstrating Google ADK and A2A interoperability for trading automation | [![Stars](https://img.shields.io/github/stars/kweinmeister/agentic-trading?style=social)](https://github.com/kweinmeister/agentic-trading) |
| [python-a2a-tutorial](https://github.com/sing1ee/python-a2a-tutorial) | [@sing1ee](https://github.com/sing1ee) | A comprehensive tutorial for implementing A2A in Python with practical examples | [![Stars](https://img.shields.io/github/stars/sing1ee/python-a2a-tutorial?style=social)](https://github.com/sing1ee/python-a2a-tutorial) |
| [a2a-python-currency](https://github.com/sing1ee/a2a-python-currency) | [@sing1ee](https://github.com/sing1ee) | A tutorial implementation of a Currency Agent using the A2A Python SDK | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-python-currency?style=social)](https://github.com/sing1ee/a2a-python-currency) |
| [a2a-mcp-openrouter](https://github.com/sing1ee/a2a-mcp-openrouter) | [@sing1ee](https://github.com/sing1ee) | Demonstrates A2A + MCP integration using OpenRouter as LLM provider, showcasing unified interface for agent-to-agent communication and tool invocation | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-mcp-openrouter?style=social)](https://github.com/sing1ee/a2a-mcp-openrouter) |
| [a2a_llama_index_file_chat](https://github.com/sing1ee/a2a_llama_index_file_chat) | [@sing1ee](https://github.com/sing1ee) | A LlamaIndex-based file chat agent supporting file upload/parsing, conversational interactions, streaming responses, and in-line citations | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a_llama_index_file_chat?style=social)](https://github.com/sing1ee/a2a_llama_index_file_chat) |

[⬆️ Back to Contents](#contents)

## Community

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first. 

[⬆️ Back to Contents](#contents) 
