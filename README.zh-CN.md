# ✨ A2A 目录 ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## 目录

- 📋 [概述](#overview)
- 🚀 [入门指南](#getting-started)
- 📚 [资源](#resources)
- 📦 [官方示例](#official-samples)
- 🛠️ [工具](#tools)
- 🤝 [社区实现](#community-implementations)
- 🎯 [社区示例](#community-samples)
- 👥 [社区](#community)
- 🤝 [贡献](#contributing)


## 概述

A2A (Agent2Agent) 是谷歌开发的开放协议，使AI代理能够安全通信和协作。它打破了孤立代理系统之间的壁垒，实现复杂的跨应用自动化。

**主要特点:**
- 🎯 简单: 使用HTTP、JSON-RPC、SSE
- 🏢 企业就绪: 注重安全性和隐私
- ⚡ 异步优先: 处理长时间运行的任务
- 🔄 模态无关: 支持文本、文件、表单、流
- 🔒 不透明执行: 代理之间交互不共享内部逻辑

**官方链接:**
- 🌐 网站: [google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub: [https://github.com/google-a2a/A2A](https://github.com/google-a2a/A2A)

## 入门指南

1. **学习基础知识**
   - 📖 阅读[技术文档](https://google.github.io/A2A/#/documentation)
   - 🎥 观看[演示视频](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **运行示例**
   - 📥 克隆[官方仓库](https://github.com/google-a2a/a2a-samples)
   - 📝 按照`/samples`中的说明操作

3. **构建自己的应用**
   - 🛠️ 使用官方库或修改示例
   - 🏗️ 从基本的A2A代理或客户端开始


## 资源

### 官方文档
- 🇺🇸 [技术文档](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON规范](https://github.com/google-a2a/A2A/tree/main/specification)
- 🇺🇸 [Agent Card规范](https://google-a2a.github.io/A2A/specification/#5-agent-discovery-the-agent-card)

## 官方示例

### Python 示例集合

#### 代理示例（基于不同框架的智能代理）

| 项目名称 | 描述 | 链接 |
|-------------|-------------|------|
| Google ADK | 费用报告填写代理，展示多轮交互和网页表单处理 | [google_adk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/google_adk) |
| AG2 + MCP | 基于AG2框架的支持MCP的代理 | [ag2](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/ag2) |
| Azure AI Foundry | 基于Azure AI Foundry服务的代理 | [azureaifoundry_sdk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/azureaifoundry_sdk) |
| LangGraph | 货币转换代理，具有工具使用和流式更新功能 | [langgraph](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/langgraph) |
| CrewAI | 图像生成代理，具有多轮交互和图像传输功能 | [crewai](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/crewai) |
| LlamaIndex | 文件解析和聊天代理，支持文件上传和流式更新 | [llama_index_file_chat](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/llama_index_file_chat) |
| Marvin | 联系信息提取代理 | [marvin](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/marvin) |
| MindsDB | 支持数据库查询的企业数据代理 | [mindsdb](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/mindsdb) |
| Semantic Kernel | 基于Microsoft Semantic Kernel框架的旅行代理 | [semantickernel](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/semantickernel) |
| AutoGen | AutoGen框架示例 | [autogen](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/autogen) |
| Hello World | 基础示例代理 | [helloworld](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/helloworld) |
| Veo Video Generation | 视频生成代理 | [veo_video_gen](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/veo_video_gen) |
| Analytics | 分析代理 | [analytics](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/analytics) |
| A2A Telemetry | 遥测数据代理 | [a2a_telemetry](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/a2a_telemetry) |
| A2A MCP | MCP协议代理 | [a2a_mcp](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/a2a_mcp) |
| Birthday Planner ADK | 生日规划代理 | [birthday_planner_adk](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/birthday_planner_adk) |
| Headless Agent Auth | 无头代理认证示例 | [headless_agent_auth](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/agents/headless_agent_auth) |

#### 主机应用（客户端应用）

| 项目名称 | 描述 | 链接 |
|-------------|-------------|------|
| CLI | 命令行客户端 | [cli](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/hosts/cli) |
| Multiagent | 多代理编排器 | [multiagent](https://github.com/google-a2a/a2a-samples/tree/main/samples/python/hosts/multiagent) |

### Go 语言示例

| 项目名称 | 描述 | 链接 |
|-------------|-------------|------|
| Server | Go语言A2A服务器实现 | [server](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/server) |
| Client | Go语言A2A客户端实现 | [client](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/client) |
| Models | 共享数据结构 | [models](https://github.com/google-a2a/a2a-samples/tree/main/samples/go/models) |

### JavaScript/TypeScript 示例

| 项目名称 | 描述 | 链接 |
|-------------|-------------|------|
| Movie Agent | 使用TMDB API的电影信息搜索代理 | [movie-agent](https://github.com/google-a2a/a2a-samples/tree/main/samples/js/src/agents/movie-agent) |
| Coder Agent | 代码生成代理 | [coder](https://github.com/google-a2a/a2a-samples/tree/main/samples/js/src/agents/coder) |



## 工具

A2A协议开发、测试和验证的必备工具。

**🔗 [A2A协议验证器](https://a2aprotocol.ai/a2a-protocol-validator)**


[⬆️ 返回目录](#contents)


## 社区实现

| 名称 | 作者 | 描述 | Stars |
|------|--------|-------------|-------|
| [a2a-python](https://github.com/google/a2a-python) | [@google](https://github.com/google) | Agent2Agent (A2A) 协议的官方Python SDK | [![Stars](https://img.shields.io/github/stars/google/a2a-python?style=social)](https://github.com/google/a2a-python) |
| [a2a-js](https://github.com/google-a2a/a2a-js) | [@google-a2a](https://github.com/google-a2a) | Agent2Agent (A2A) 协议的官方JavaScript SDK - 帮助运行遵循A2A协议的代理应用程序的JavaScript库 | [![Stars](https://img.shields.io/github/stars/google-a2a/a2a-js?style=social)](https://github.com/google-a2a/a2a-js) |
| [a2ajava](https://github.com/vishalmysore/a2ajava) | [@vishalmysore](https://github.com/vishalmysore) | 为Spring Boot应用提供的纯Java实现的谷歌A2A协议，包含客户端和服务器端实现 | [![Stars](https://img.shields.io/github/stars/vishalmysore/a2ajava?style=social)](https://github.com/vishalmysore/a2ajava) |
| [a2a4j](https://github.com/a2ap/a2a4j) | [@a2ap](https://github.com/a2ap) | A2A4J 是 Agent2Agent 协议的全面 Java 实现，为独立的 AI 代理系统之间的通信和互操作性提供了一个开放标准。 | [![Stars](https://img.shields.io/github/stars/a2ap/a2a4j?style=social)](https://github.com/a2ap/a2a4j) |
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | 注重模块化和可扩展性的TypeScript A2A协议实现 | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [trpc-a2a-go](https://github.com/trpc-group/trpc-a2a-go) | [@trpc-group](https://github.com/trpc-group) | tRPC团队的Go A2A实现，具有完整的客户端/服务器支持、内存任务管理、流式响应、会话管理、多种认证方法（JWT、API Key、OAuth2）和全面的示例 | [![Stars](https://img.shields.io/github/stars/trpc-group/trpc-a2a-go?style=social)](https://github.com/trpc-group/trpc-a2a-go) |
| [jira-a2a](https://github.com/tuannvm/jira-a2a) | [@tuannvm](https://github.com/tuannvm) | Jira A2A系统是一个使用tRPC-A2A-Go框架的DevOps工作流自动化平台。它由独立的Go代理组成，这些代理通过A2A消息进行通信。 | [![Stars](https://img.shields.io/github/stars/tuannvm/jira-a2a?style=social)](https://github.com/tuannvm/jira-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | 用于构建A2A服务器的Go库，附带示例实现 | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | 遵循六边形架构原则的惯用Rust实现 | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | 用于A2A通信的极简Python SDK | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A2A协议的C#/.NET实现 | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | 用于将A2A协议集成到NestJS应用程序的模块 | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | 用于实现A2A协议的易用Python库 | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 用于托管、注册、发现和与代理交互的A2A网络实现 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 基于谷歌ADK构建的AI代理开发框架，促进潜在用于A2A网络的代理创建 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | 轻量级的A2A Python实现 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A2A的命令行客户端 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A测试套件](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A测试套件 | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | 内置MCP和A2A支持的自托管浏览器代理 | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | 支持MCP的多代理聊天应用，旨在通过A2A协议暴露代理并作为客户端连接到远程A2A代理 | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | 专注于开发者体验和全面功能的Agent2Agent协议JS/TS SDK | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |
| [a2a-validation-tool](https://github.com/llmx-de/a2a-validation-tool) | [@llmx-de](https://github.com/llmx-de) | 用于测试和验证Agent-to-Agent (A2A)协议实现的桌面应用程序 | [![Stars](https://img.shields.io/github/stars/llmx-de/a2a-validation-tool?style=social)](https://github.com/llmx-de/a2a-validation-tool) |

[⬆️ 返回目录](#contents)


### 社区示例

| 名称 | 作者 | 描述 | Stars |
|------|--------|-------------|-------|
| [a2a-agent-coder](https://github.com/sing1ee/a2a-agent-coder) | [@sing1ee](https://github.com/sing1ee) | 带有A2A服务器和客户端的Coder Agent实现 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-agent-coder?style=social)](https://github.com/sing1ee/a2a-agent-coder) |
| [agentic-trading](https://github.com/kweinmeister/agentic-trading) | [@kweinmeister](https://github.com/kweinmeister) | 展示Google ADK和A2A互操作性的交易自动化示例应用 | [![Stars](https://img.shields.io/github/stars/kweinmeister/agentic-trading?style=social)](https://github.com/kweinmeister/agentic-trading) |
| [python-a2a-tutorial](https://github.com/sing1ee/python-a2a-tutorial) | [@sing1ee](https://github.com/sing1ee) | 包含实践示例的Python A2A实现综合教程 | [![Stars](https://img.shields.io/github/stars/sing1ee/python-a2a-tutorial?style=social)](https://github.com/sing1ee/python-a2a-tutorial) |
| [a2a-python-currency](https://github.com/sing1ee/a2a-python-currency) | [@sing1ee](https://github.com/sing1ee) | 使用A2A Python SDK的货币代理教程实现 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-python-currency?style=social)](https://github.com/sing1ee/a2a-python-currency) |
| [a2a-mcp-openrouter](https://github.com/sing1ee/a2a-mcp-openrouter) | [@sing1ee](https://github.com/sing1ee) | 演示使用OpenRouter作为LLM提供商的A2A + MCP集成，展示代理间通信和工具调用的统一接口 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-mcp-openrouter?style=social)](https://github.com/sing1ee/a2a-mcp-openrouter) |
| [a2a_llama_index_file_chat](https://github.com/sing1ee/a2a_llama_index_file_chat) | [@sing1ee](https://github.com/sing1ee) | 基于LlamaIndex的文件聊天代理，支持文件上传/解析、对话交互、流式响应和内联引用 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a_llama_index_file_chat?style=social)](https://github.com/sing1ee/a2a_llama_index_file_chat) |

[⬆️ 返回目录](#contents)

## 社区

- 🐛 [GitHub问题](https://github.com/google/A2A/issues)
- 💬 [GitHub讨论](https://github.com/google/A2A/discussions/)

## 贡献

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。

[⬆️ 返回目录](#contents)
