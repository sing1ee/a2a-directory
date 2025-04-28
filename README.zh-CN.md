# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## 目录

- 📋 [概述](#overview)
- 🚀 [入门指南](#getting-started)
- 📚 [资源](#resources)
- 💻 [实现](#implementations)
- 🎴 [AgentCard](#agentcard)
- 🤝 [社区实现](#community-implementations)
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
- 📦 GitHub: [github.com/google/A2A](https://github.com/google/A2A)

## 入门指南

1. **学习基础知识**
   - 📖 阅读[技术文档](https://google.github.io/A2A/#/documentation)
   - 🎥 观看[演示视频](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **运行示例**
   - 📥 克隆[官方仓库](https://github.com/google/A2A)
   - 📝 按照`/samples`中的说明操作

3. **构建自己的应用**
   - 🛠️ 使用官方库或修改示例
   - 🏗️ 从基本的A2A代理或客户端开始


## 资源

### 官方文档
- 🇺🇸 [技术文档](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON规范](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [Agent Card规范](https://google.github.io/A2A/#/documentation?id=agent-card)

### 社区文档
- 🇺🇸 [A2A TypeScript指南](docs/a2a-typescript-guide.md) - 在TypeScript中实现A2A的综合指南
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - A2A与Model Context Protocol的比较
- 🇺🇸 [理解A2A协议](docs/understanding-a2a-protocol.md) - 深入了解A2A协议概念
- 🇺🇸 [A2A示例方法和JSON响应](docs/a2a-sample-methods-and-json-responses.md) - A2A方法和响应的详细示例
- 🇺🇸 [Python A2A](docs/python-a2a.md): 一个强大且易用的库，用于实现谷歌的[Agent-to-Agent (A2A)协议](https://google.github.io/A2A/) - [链接](https://a2aprotocol.ai/blog/python-a2a)
- 🇨🇳 [A2A 协议介绍](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A 协议的中文介绍

## 论文

- 📄 [AI Agent 协议综述](https://arxiv.org/pdf/2504.16736) - 一篇学术论文，调查了现有的 LLM agent 通信协议（包括 A2A 所属的类别），对它们进行分类，分析性能，并讨论未来挑战。

[⬆️ 返回目录](#contents)

## 实现

### 官方示例

#### Python
- 🐍 **通用库**: 核心HTTP、JSON-RPC、SSE处理 - [链接](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **主机(客户端)**: 命令行客户端示例 - [链接](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **主机(代理)**: 委托给A2A代理的编排代理 - [链接](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **服务器库**: 核心服务器实现 - [链接](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **客户端库**: 客户端实现 - [链接](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **主机(客户端)**: 命令行客户端示例 - [链接](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

## 社区实现

| 名称 | 作者 | 描述 | 星标 |
|------|--------|-------------|-------|
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | A2A协议的TypeScript实现，注重模块化和可扩展性 | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | 用于构建A2A服务器的Go库，附带示例实现 | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | 遵循六边形架构原则的惯用Rust实现 | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | 用于A2A通信的极简Python SDK | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A2A协议的C#/.NET实现 | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | 用于将A2A协议集成到NestJS应用程序的模块 | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | 用于实现A2A协议的易用Python库 | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 用于托管、注册、发现和与代理交互的A2A网络实现 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 基于谷歌ADK构建的AI代理开发框架，促进潜在用于A2A网络的代理创建 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | 一个轻量级的 A2A Python 实现 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A2A的命令行客户端 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A 测试套件](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A 测试套件 | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | 一个内置 MCP 和 A2A 支持的自托管浏览器代理 | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | 一个支持 MCP 的多智能体聊天应用，旨在通过 A2A 协议暴露智能体并作为客户端连接到远程 A2A 智能体 | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | 一个专注于开发者体验和全面功能的 Agent2Agent 协议 JS/TS SDK | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |

[⬆️ 返回目录](#contents)

### 框架集成

#### Python
- 🐍 **LangGraph**: 货币转换(特性: 工具、流式处理、多轮对话) - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**: 图像生成(特性: 非文本工件(文件)) - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**: 费用报销(特性: 多轮对话、表单(DataPart)) - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**: 用于实现谷歌[Agent-to-Agent (A2A)协议](https://google.github.io/A2A/)的强大且易用的库 - [链接](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**: 电影信息/代码生成(特性: 工具、工件(文件)、异步) - [链接](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### 社区示例

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**: 具有A2A服务器和客户端的Coder代理实现 - [链接](https://github.com/sing1ee/a2a-agent-coder)

[⬆️ 返回目录](#contents)

## AgentCard

## 社区

- 🐛 [GitHub问题](https://github.com/google/A2A/issues)
- 💬 [GitHub讨论](https://github.com/google/A2A/discussions/)

## 贡献

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。