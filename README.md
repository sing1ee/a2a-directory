# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

<a id="contents"></a>
## Contents

- 📋 [Overview](#overview)
- 🚀 [Getting Started](#getting-started)
- 📚 [Resources](#resources)
- 📦 [Official Samples](#official-samples)
- 🛠️ [Tools](#tools)
- 🤝 [Community Implementations](#community-implementations)
- 🎯 [Community Samples](#community-samples)
- 🤖 [A2A-Compatible Services](#a2a-compatible-services)
- 💰 [x402-Enabled Services](#x402-enabled-services)
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

### Community Documentation
- 🇺🇸 [A2A TypeScript Guide](docs/a2a-typescript-guide.md) — Comprehensive guide to implementing A2A in TypeScript
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) — Comparison of A2A and the Model Context Protocol
- 🇺🇸 [Understanding the A2A Protocol](docs/understanding-a2a-protocol.md) — Deep dive into A2A protocol concepts
- 🇺🇸 [A2A Sample Methods and JSON Responses](docs/a2a-sample-methods-and-json-responses.md) — Detailed examples of A2A methods and JSON responses
- 🇺🇸 [Python A2A](docs/python-a2a.md) — Comprehensive guide to Google's Agent-to-Agent Protocol in Python
- 🇺🇸 [A2A BeeAI Integration](docs/a2a-beeai-integration.md) — Integrating the A2A protocol with the BeeAI Framework
- 🇺🇸 [A2A Implementations](docs/a2a-implementations.md) — A community-maintained list of A2A implementations

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

Production A2A agents, services, and tools for development, testing, and validation.

| Name | Author | Description | Stars |
|------|--------|-------------|-------|
| [A2A Protocol Validator](https://a2aprotocol.ai/a2a-protocol-validator) | [a2aprotocol.ai](https://a2aprotocol.ai) | Validate A2A protocol implementations. | N/A |
| [Not Human Search](https://nothumansearch.ai) | [@unitedideas](https://github.com/unitedideas) | Agent discovery search engine. Indexes 8,000+ agent-readable services ranked across 7 signals (llms.txt, OpenAPI, ai-plugin, MCP, structured API, robots.txt, schema.org). Includes `verify_mcp` live JSON-RPC probe to confirm an advertised agent endpoint is actually reachable. Queryable via REST API, MCP server, or browser. | [![Stars](https://img.shields.io/github/stars/unitedideas/nothumansearch?style=social)](https://github.com/unitedideas/nothumansearch) |
| [TrustBoost PII Sanitizer](https://api.trustboost.dev) | [@teodorofodocrispin-cmyk](https://github.com/teodorofodocrispin-cmyk) | Production PII sanitization layer for autonomous AI agent pipelines. Redacts emails, national IDs, API keys, and financial data before text reaches LLMs. Every paid sanitization anchored on Solana — verifiable at `/verify/{anchor_tx}`. 8 languages: EN, ES-LATAM, PT-BR, DE, JA, FR, IT, KO. x402 compatible, MCP native, EU AI Act compliant. [Agent Card](https://api.trustboost.dev/.well-known/agent-card.json) \| [llms.txt](https://api.trustboost.dev/llms.txt) | [![Stars](https://img.shields.io/github/stars/teodorofodocrispin-cmyk/TrustBoost-PII-Sanitizer?style=social)](https://github.com/teodorofodocrispin-cmyk/TrustBoost-PII-Sanitizer) |
| [Ambr](https://ambr.run) | [OMRA Corp](https://ambr.run) | Production A2A agent for legal contract management. Creates, signs, and verifies dual-format Ricardian Contracts (human-readable + machine-parsable JSON, SHA-256 linked). 6 skills, x402 USDC payments. [Agent Card](https://getamber.dev/.well-known/agent.json) | N/A |
| [AlgoVoi](https://algovoi.co.uk) | [AlgoVoi](https://algovoi.co.uk) | Production multi-chain, multi-protocol A2A payment gateway. Verifies on-chain payments and creates hosted checkout links across 7 chains (Algorand, VOI, Hedera, Stellar, Base, Solana, Tempo). Supports x402, MPP (IETF), and AP2 (Google Agentic Payments) on a single endpoint. 4 skills: verify-payment, create-checkout, check-status, post-twitter-checkout. [Agent Card](https://api1.ilovechicken.co.uk/.well-known/agent.json) | N/A |
| [HiveAttest](https://github.com/srotzin/hive-mcp-attest) | [@srotzin](https://github.com/srotzin) | Production A2A v0.3.0 agent for pre-action verification. Issues Ed25519-signed C18 receipts on every gate decision (allow AND deny), real-rail USDC settlement on Base, and machine-verifiable [Agent Card](https://thehiveryiq.com/.well-known/agent.json). Live demo: https://thehiveryiq.com/attest-demo.html | [![Stars](https://img.shields.io/github/stars/srotzin/hive-mcp-attest?style=social)](https://github.com/srotzin/hive-mcp-attest) |
| [Rosentic](https://rosentic.com) | [Rosentic](https://rosentic.com) | Deterministic cross-branch semantic conflict detection for merge safety. Checks active git branches for function signature mismatches, HTTP route conflicts, GraphQL breaks, OpenAPI drift, and protobuf contract changes across 15+ languages. 5 skills: assess-posture, check-conflicts, explain-conflict, list-branches, merge-index. [Agent Card](https://api.rosentic.com/.well-known/agent.json) | [![Stars](https://img.shields.io/github/stars/Rosentic/rosentic-action?style=social)](https://github.com/Rosentic/rosentic-action) |
| [Agent Ready](https://agent-ready.dev) | [Agent Ready](https://agent-ready.dev) | Production A2A v0.3.0 agent that scores any public URL 0–100 for AI-agent readability against the Vercel Agent Readability Spec, llmstxt.org, and agent-protocol manifests, with per-check fixes. 3 skills (scan_site, get_scan, ask) over JSON-RPC at /api/v1/a2a — bearer-auth scans, public NLWeb ask. [Agent Card](https://agent-ready.dev/.well-known/agent-card.json) | N/A |
| [Numbers Online](https://numbers.online) | [Numbers Online](https://numbers.online) | Production A2A v0.3.0 agent for phone-number intelligence. 4 skills (phone_lookup, line_type, caller_risk, dnc_check) over JSON-RPC at /api/v1/a2a — bearer-auth — returning line type, range carrier, country, CNAM, STIR/SHAKEN verstat, a labeled spam-risk signal, and a first-party do-not-contact (DNC) signal, each a supplementary low-confidence signal, with Ed25519-signed receipts. [Agent Card](https://numbers.online/.well-known/agent-card.json) | N/A |
| [Merchant-0](https://merchant-0.com) | [@RaulA3](https://github.com/RaulA3) | Production autonomous A2A commerce agent for SEA and ASEAN trade intelligence. Grok-4.3 + live web search intel queries ($2.39/query, 20% new-agent discount), SEA regulatory compliance briefs, and subscription plans ($49/month). Full AP2 protocol: discover → negotiate → sign → execute. Free trial: one query per agent DID. [Agent Card](https://merchant-0.com/.well-known/agent.json) \| [Subscribe](https://merchant-0.com/subscribe) | N/A |
| [Relm](https://relmcrm.com) | [Relm](https://relmcrm.com) | Hosted, API-first CRM for LLMs and AI agents. Native A2A endpoint at api.relmcrm.com/a2a (JSON-RPC 2.0), plus REST + MCP, so agents create/update contacts, companies, deals and notes as shared memory. [Agent Card](https://relmcrm.com/.well-known/agent-card.json) | N/A |
| [risk-api](https://github.com/JleviEderer/risk-api) | [@JleviEderer](https://github.com/JleviEderer) | Smart contract risk scoring agent for EVM chains. Analyzes bytecode patterns, proxy structures, and deployer reputation via A2A protocol with x402 payments ($0.10/query). Live at [risk-api.life.conway.tech](https://risk-api.life.conway.tech) | [![Stars](https://img.shields.io/github/stars/JleviEderer/risk-api?style=social)](https://github.com/JleviEderer/risk-api) |
| [openstoa](https://github.com/zkproofport/openstoa) | [@zkproofport](https://github.com/zkproofport) | ZK-gated community where humans and AI agents coexist. Agents authenticate via Google OIDC zero-knowledge proofs and join topic discussions. Hosts A2A agent card at `/.well-known/agent-card.json`. 🏅 1st Place at The Synthesis Hackathon (Agents That Keep Secrets, April 2026, 506 projects). Live at [openstoa.xyz](https://www.openstoa.xyz) | [![Stars](https://img.shields.io/github/stars/zkproofport/openstoa?style=social)](https://github.com/zkproofport/openstoa) |
| [proofport-ai](https://github.com/zkproofport/proofport-ai) | [@zkproofport](https://github.com/zkproofport) | Server-side ZK proof generation MCP server with A2A agent card. Generates Coinbase KYC, Country, OIDC, Workspace, MS 365 proofs. AWS Nitro Enclave TEE proving, ERC-8004 registered (token ID 25331), x402 USDC payments on Base | [![Stars](https://img.shields.io/github/stars/zkproofport/proofport-ai?style=social)](https://github.com/zkproofport/proofport-ai) |
| [AgentServices](https://agentservices.to) | [@vbkotecha](https://github.com/vbkotecha) | Production A2A agent marketplace with 54 services — market intelligence, onchain data, FX rates, bundled synthesis, and inference. x402 USDC micropayments on Base, MCP server (37 tools), and agent-card discovery at `/.well-known/agent.json`. Indexed on Agenstry and the official MCP Registry. | [![Stars](https://img.shields.io/github/stars/vbkotecha/aiservices-api?style=social)](https://github.com/vbkotecha/aiservices-api) |
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
| [Agent Reputation (Agent Hub)](https://agentreputation.dev) | [@SamyTouri](https://github.com/SamyTouri) | Live cross-registry discovery & reputation service: semantic search over 15,000+ listed agents and MCP servers, 0-5 ratings split native vs imported, A2A agent card + remote MCP endpoint, no auth required, chartered by a public constitution | [![Stars](https://img.shields.io/github/stars/SamyTouri/agent-hub?style=social)](https://github.com/SamyTouri/agent-hub) |
| [Bindu](https://github.com/getbindu/Bindu) | [@getbindu](https://github.com/getbindu) | Production runtime for A2A-compatible agents. Wrap agents built with LangChain, Agno, CrewAI, OpenAI SDK, or plain code using `bindufy()` to add DID identity, OAuth2 authentication, X402 payments, retries, observability, push notifications, storage, scheduling, and gRPC-based multi-language support across Python, TypeScript, and Kotlin. | [![Stars](https://img.shields.io/github/stars/getbindu/Bindu?style=social)](https://github.com/getbindu/Bindu) |
| [A2A Nexus](https://github.com/jinwon-int/a2a-nexus) | [@jinwon-int](https://github.com/jinwon-int) | Public alpha A2A task/evidence control plane for broker-managed worker registration, auditable task lifecycle evidence, source-only review bridges, isolated patch execution, and finalizer-oriented closeout reports. Not affiliated with or endorsed by a2aproject. | [![Stars](https://img.shields.io/github/stars/jinwon-int/a2a-nexus?style=social)](https://github.com/jinwon-int/a2a-nexus) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | An AI agent development framework built on Google's ADK, facilitating agent creation potentially for A2A networks | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | A lightweight A2A python implementation | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A command-line client for the A2A | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A Test Suit](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A Test Suite | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | A Self-hosted Browser Using Agent with built-in MCP and A2A support | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | A multi-agent chat application with MCP support, aiming to expose agents via the A2A protocol and connect to remote A2A agents as a client | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | A JS/TS SDK for the Agent2Agent Protocol with a focus on developer experience and comprehensive features | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |
| [a2a-validation-tool](https://github.com/llmx-de/a2a-validation-tool) | [@llmx-de](https://github.com/llmx-de) | A desktop application for testing and validating Agent-to-Agent (A2A) protocol implementations | [![Stars](https://img.shields.io/github/stars/llmx-de/a2a-validation-tool?style=social)](https://github.com/llmx-de/a2a-validation-tool) |
| [Protolink](https://github.com/nMaroulis/protolink) | [@nMaroulis](https://github.com/nMaroulis) | A Python library for building autonomous Agents with Agent-to-Agent (A2A) protocol implementations, integrating LLMs and tools. | [![Stars](https://img.shields.io/github/stars/nMaroulis/protolink?style=social)](https://github.com/nMaroulis/protolink) |
| [OpenAgents](https://github.com/openagents-org/openagents) | [@openagents-org](https://github.com/openagents-org) | Open-source platform for building AI agent networks with A2A, MCP, WebSocket, gRPC, and HTTP support | [![Stars](https://img.shields.io/github/stars/openagents-org/openagents?style=social)](https://github.com/openagents-org/openagents) |
| [systemprompt-template](https://github.com/systempromptio/systemprompt-template) | [@Ejb503](https://github.com/Ejb503) | Production Rust A2A + MCP governance runtime. Single compiled binary that authenticates, authorises, rate-limits, logs, and costs every AI interaction. Ships with A2A v0.3.0 agent cards, OAuth2 security, streaming support, and 40+ scripted demos. Self-hosted, air-gap capable. | [![Stars](https://img.shields.io/github/stars/systempromptio/systemprompt-template?style=social)](https://github.com/systempromptio/systemprompt-template) |
| [humanbrowser](https://github.com/VirixLabs/humanbrowser) | [@VirixLabs](https://github.com/VirixLabs) | A2A 1.0 cloud-Chromium agent for AI clients. Drives a stealth browser engine with residential proxies and built-in captcha solving over a single A2A endpoint, with an open-source SDK (`@virixlabs/humanbrowser`), an MCP server (`npx -y @virixlabs/humanbrowser mcp`), and a hosted card at [agent.humanbrowser.cloud](https://agent.humanbrowser.cloud/.well-known/agent-card.json). Apache-2.0. | [![Stars](https://img.shields.io/github/stars/VirixLabs/humanbrowser?style=social)](https://github.com/VirixLabs/humanbrowser) |
| [agenda-intelligence-md](https://github.com/vassiliylakhonin/agenda-intelligence-md) | [@vassiliylakhonin](https://github.com/vassiliylakhonin) | Evidence-discipline runtime for strategic-risk agents over one core service layer (MCP, HTTP, A2A, Cloudflare Worker). Ships A2A vertical workers — Middle Corridor deal-risk gate, CIS secondary-sanctions exposure, agentic interaction trust — that turn a partial evidence pack into a structured triage with evidence gaps, a decision-readiness score, and mandatory human review. Pre-compliance evidence triage only; not legal or sanctions advice; no factual-truth verification. | [![Stars](https://img.shields.io/github/stars/vassiliylakhonin/agenda-intelligence-md?style=social)](https://github.com/vassiliylakhonin/agenda-intelligence-md) |
[⬆️ Back to Contents](#contents)


## Community Samples

| Name | Author | Description | Stars |
|------|--------|-------------|-------|
| [a2a-agent-coder](https://github.com/sing1ee/a2a-agent-coder) | [@sing1ee](https://github.com/sing1ee) | A Coder Agent implementation with A2A Server and Client | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-agent-coder?style=social)](https://github.com/sing1ee/a2a-agent-coder) |
| [agentic-trading](https://github.com/kweinmeister/agentic-trading) | [@kweinmeister](https://github.com/kweinmeister) | A sample application demonstrating Google ADK and A2A interoperability for trading automation | [![Stars](https://img.shields.io/github/stars/kweinmeister/agentic-trading?style=social)](https://github.com/kweinmeister/agentic-trading) |
| [python-a2a-tutorial](https://github.com/sing1ee/python-a2a-tutorial) | [@sing1ee](https://github.com/sing1ee) | A comprehensive tutorial for implementing A2A in Python with practical examples | [![Stars](https://img.shields.io/github/stars/sing1ee/python-a2a-tutorial?style=social)](https://github.com/sing1ee/python-a2a-tutorial) |
| [a2a-python-currency](https://github.com/sing1ee/a2a-python-currency) | [@sing1ee](https://github.com/sing1ee) | A tutorial implementation of a Currency Agent using the A2A Python SDK | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-python-currency?style=social)](https://github.com/sing1ee/a2a-python-currency) |
| [a2a-mcp-openrouter](https://github.com/sing1ee/a2a-mcp-openrouter) | [@sing1ee](https://github.com/sing1ee) | Demonstrates A2A + MCP integration using OpenRouter as LLM provider, showcasing unified interface for agent-to-agent communication and tool invocation | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-mcp-openrouter?style=social)](https://github.com/sing1ee/a2a-mcp-openrouter) |
| [a2a_llama_index_file_chat](https://github.com/sing1ee/a2a_llama_index_file_chat) | [@sing1ee](https://github.com/sing1ee) | A LlamaIndex-based file chat agent supporting file upload/parsing, conversational interactions, streaming responses, and in-line citations | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a_llama_index_file_chat?style=social)](https://github.com/sing1ee/a2a_llama_index_file_chat) |
| [a2a-mcp-bridge](https://github.com/GipsyChef/a2a-mcp-bridge) | [@GipsyChef](https://github.com/GipsyChef) | Two Claude agents collaborating locally over A2A (agent-to-agent) and MCP (tools), with Claude on Vertex AI. A runnable Researcher + Analyst reference that also works as an MCP skill for Claude Code, Codex, and opencode. | [![Stars](https://img.shields.io/github/stars/GipsyChef/a2a-mcp-bridge?style=social)](https://github.com/GipsyChef/a2a-mcp-bridge) |
[⬆️ Back to Contents](#contents)


## A2A Agents

Hosted services and production agents that expose an A2A Agent Card or a native A2A endpoint. Each also appears in its primary section — collected here for discoverability by capability.

| Name | A2A Agent Card / Endpoint |
|------|---------------------------|
| [TrustBoost PII Sanitizer](https://api.trustboost.dev) | [Agent Card](https://api.trustboost.dev/.well-known/agent-card.json) |
| [Ambr](https://ambr.run) | [Agent Card](https://getamber.dev/.well-known/agent.json) |
| [AlgoVoi](https://algovoi.co.uk) | [Agent Card](https://api1.ilovechicken.co.uk/.well-known/agent.json) |
| [HiveAttest](https://github.com/srotzin/hive-mcp-attest) | [Agent Card](https://thehiveryiq.com/.well-known/agent.json) |
| [Rosentic](https://rosentic.com) | [Agent Card](https://api.rosentic.com/.well-known/agent.json) |
| [Agent Ready](https://agent-ready.dev) | [Agent Card](https://agent-ready.dev/.well-known/agent-card.json) |
| [Numbers Online](https://numbers.online) | [Agent Card](https://numbers.online/.well-known/agent-card.json) |
| [Merchant-0](https://merchant-0.com) | [Agent Card](https://merchant-0.com/.well-known/agent.json) |
| [Relm](https://relmcrm.com) | [Agent Card](https://relmcrm.com/.well-known/agent-card.json) · endpoint `api.relmcrm.com/a2a` |
| [risk-api](https://github.com/JleviEderer/risk-api) | A2A endpoint · [live](https://risk-api.life.conway.tech) |
| [openstoa](https://github.com/zkproofport/openstoa) | Agent card at `/.well-known/agent-card.json` · [live](https://www.openstoa.xyz) |
| [proofport-ai](https://github.com/zkproofport/proofport-ai) | A2A agent card |
| [AgentServices](https://agentservices.to) | Agent card at `/.well-known/agent.json` |
| [Agent Reputation (Agent Hub)](https://agentreputation.dev) | A2A agent card + remote MCP endpoint |
| [humanbrowser](https://github.com/VirixLabs/humanbrowser) | [Hosted card](https://agent.humanbrowser.cloud/.well-known/agent-card.json) |
| [Money You're Owed](https://moneyyoureowed.com) | [Agent Card](https://agent.moneyyoureowed.com/.well-known/agent-card.json) |
[⬆️ Back to Contents](#contents)


## x402-Enabled Services

Services that accept x402 (HTTP 402 Payment Required) payments — typically USDC on Base. Each also appears in its primary section — collected here for discoverability by capability.

| Name | x402 Details |
|------|--------------|
| [TrustBoost PII Sanitizer](https://api.trustboost.dev) | x402 compatible; payments anchored on Solana |
| [Ambr](https://ambr.run) | x402 USDC payments |
| [AlgoVoi](https://algovoi.co.uk) | x402 (also MPP, AP2) on a single endpoint |
| [risk-api](https://github.com/JleviEderer/risk-api) | x402 payments, $0.10/query |
| [proofport-ai](https://github.com/zkproofport/proofport-ai) | x402 USDC payments on Base |
| [AgentServices](https://agentservices.to) | x402 USDC micropayments on Base |
| [Bindu](https://github.com/getbindu/Bindu) | X402 payments via `bindufy()` runtime |
[⬆️ Back to Contents](#contents)


## Community

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first. 

[⬆️ Back to Contents](#contents)
