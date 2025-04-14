# ✨ Agent2Agent 协议 ✨

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md)

## 目录

- 📋 [概述](#概述)
- 🚀 [快速开始](#快速开始)
- 📚 [资源](#资源)
- 💻 [实现](#实现)
- 🎴 [AgentCard](#agentcard)
- 👥 [社区](#社区)
- 🤝 [贡献](#贡献)

## 概述

A2A (Agent2Agent) 是 Google 推出的一个开放协议，使 AI 智能体能够安全地通信和协作。它打破了孤立智能体系统之间的壁垒，实现了复杂的跨应用自动化。

**主要特性：**
- 🎯 简单：使用 HTTP、JSON-RPC、SSE
- 🏢 企业级：注重安全性和隐私
- ⚡ 异步优先：处理长时间运行的任务
- 🔄 模态无关：支持文本、文件、表单、流
- 🔒 不透明执行：智能体交互时不共享内部逻辑

**官方链接：**
- 🌐 网站：[google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub：[github.com/google/A2A](https://github.com/google/A2A)

## 快速开始

1. **学习基础知识**
   - 📖 阅读[技术文档](https://google.github.io/A2A/#/documentation)
   - 🎥 观看[演示视频](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **运行示例**
   - 📥 克隆[官方仓库](https://github.com/google/A2A)
   - 📝 按照 `/samples` 目录中的说明操作

3. **构建自己的实现**
   - 🛠️ 使用官方库或改编示例
   - 🏗️ 从基本的 A2A 智能体或客户端开始

## 资源

### 官方文档
- 🇺🇸 [技术文档](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON 规范](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [智能体卡片规范](https://google.github.io/A2A/#/documentation?id=agent-card)

### 社区文档
- 🇺🇸 [A2A TypeScript 指南](docs/a2a-typescript-guide.md) - TypeScript 实现 A2A 的全面指南
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - A2A 和模型上下文协议的比较
- 🇺🇸 [理解 A2A 协议](docs/understanding-a2a-protocol.md) - 深入探讨 A2A 协议概念
- 🇺🇸 [A2A 示例方法和 JSON 响应](docs/a2a-sample-methods-and-json-responses.md) - A2A 方法和响应的详细示例
- 🇺🇸 [Python A2A：Google Agent-to-Agent 协议全面指南](docs/python-a2a.md) - Python A2A 是一个强大且易用的库，用于实现 Google 的 [Agent-to-Agent (A2A) 协议](https://google.github.io/A2A/)
- 🇨🇳 [A2A 协议介绍](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A 协议的中文介绍

## 实现

### 官方示例

#### Python
- 🐍 **通用库**：核心 HTTP、JSON-RPC、SSE 处理 - [链接](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **主机（客户端）**：命令行客户端示例 - [链接](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **主机（智能体）**：协调多个 A2A 智能体的编排器 - [链接](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **服务器库**：核心服务器实现 - [链接](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **客户端库**：客户端实现 - [链接](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **主机（客户端）**：命令行客户端示例 - [链接](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

### 框架集成

#### Python
- 🐍 **LangGraph**：货币转换（特性：工具、流式处理、多轮对话） - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**：图像生成（特性：非文本工件（文件）） - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**：费用报销（特性：多轮对话、表单（DataPart）） - [链接](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**：一个强大且易用的库，用于实现 Google 的 [Agent-to-Agent (A2A) 协议](https://google.github.io/A2A/) - [链接](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**：电影信息/代码生成（特性：工具、工件（文件）、异步） - [链接](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### 社区示例

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**：带有 A2A 服务器和客户端的编码器智能体实现 - [链接](https://github.com/sing1ee/a2a-agent-coder)

## AgentCard

## 社区

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## 贡献

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。 