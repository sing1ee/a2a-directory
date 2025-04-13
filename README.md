# ✨ Agent2Agent Protocol ✨

![a2aprotocol.ai](/images/a2a-protocol.png)

![PR Welcome](/images/prs-welcome.svg)

## Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Resources](#resources)
- [Implementations](#implementations)
- [Community](#community)
- [Contributing](#contributing)

## Overview

A2A (Agent2Agent) is an open protocol from Google enabling AI agents to communicate securely and collaborate. It breaks down silos between isolated agent systems, allowing for complex cross-application automation.

**Key Features:**
- Simple: Uses HTTP, JSON-RPC, SSE
- Enterprise Ready: Focuses on security and privacy
- Async First: Handles long-running tasks
- Modality Agnostic: Supports text, files, forms, streams
- Opaque Execution: Agents interact without sharing internal logic

**Official Links:**
- Website: [google.github.io/A2A](https://google.github.io/A2A)
- GitHub: [github.com/google/A2A](https://github.com/google/A2A)

## Getting Started

1. **Learn the Basics**
   - Read the [technical documentation](https://google.github.io/A2A/#/documentation)
   - Watch the [demo video](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **Run Samples**
   - Clone the [official repo](https://github.com/google/A2A)
   - Follow instructions in `/samples`

3. **Build Your Own**
   - Use official libraries or adapt samples
   - Start with a basic A2A agent or client

## Resources

### Official Documentation
- [Technical Documentation](https://google.github.io/A2A/#/documentation)
- [JSON Specification](https://github.com/google/A2A/tree/main/specification/json)
- [Agent Card Specification](https://google.github.io/A2A/#/documentation?id=agent-card)

### Related Protocols
- [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol/servers)

## Implementations

### Official Samples
| Language | Type | Description | Link |
|----------|------|-------------|------|
| Python | Common Library | Core HTTP, JSON-RPC, SSE handling | [Link](https://github.com/google/A2A/tree/main/samples/python/common) |
| Python | CLI Client | Command-line client example | [Link](https://github.com/google/A2A/tree/main/samples/python/hosts/cli) |
| JS/TS | Server Library | Core server implementation | [Link](https://github.com/google/A2A/tree/main/samples/js/src/server) |

### Framework Integrations
| Framework | Description | Link |
|-----------|-------------|------|
| LangGraph | Currency conversion agent | [Link](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph) |
| CrewAI | Image generation agent | [Link](https://github.com/google/A2A/tree/main/samples/python/agents/crewai) |
| Genkit | Movie info / Code generation | [Link](https://github.com/google/A2A/tree/main/samples/js/src/agents) |

## Community

- [GitHub Issues](https://github.com/google/A2A/issues)
- [GitHub Discussions](https://github.com/google/A2A/discussions/)
- [Feedback Form](https://docs.google.com/forms/d/e/1FAIpQLScS23OMSKnVFmYeqS2dP7dxY3eTyT7lmtGLUa8OJZfP4RTijQ/viewform)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first. 