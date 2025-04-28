# ✨ A2A 目錄 ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md) | [繁體中文](README.zh-TW.md) | [香港繁體](README.zh-HK.md)

<a id="contents"></a>
## 目錄

- 📋 [概覽](#概覽)
- 🚀 [入門指南](#入門指南)
- 📚 [資源](#資源)
- 💻 [實現方案](#實現方案)
- 🎴 [AgentCard](#agentcard)
- 🤝 [社區實現](#社區實現)
- 👥 [社區](#社區)
- 🤝 [貢獻](#貢獻)


## 概覽

A2A (Agent2Agent) 係 Google 推出嘅開放協議，令 AI 代理能夠安全地通訊同埋協作。佢打破咗隔離代理系統之間嘅壁壘，實現複雜嘅跨應用自動化。

**主要特點：**
- 🎯 簡單：使用 HTTP、JSON-RPC、SSE
- 🏢 企業級：注重安全性同私隱
- ⚡ 非同步優先：處理長時間運行嘅任務
- 🔄 模態不可知：支援文字、檔案、表單、串流
- 🔒 不透明執行：代理互動而唔需要共享內部邏輯

**官方連結：**
- 🌐 網站：[google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub：[github.com/google/A2A](https://github.com/google/A2A)

## 入門指南

1. **學習基礎知識**
   - 📖 閱讀[技術文檔](https://google.github.io/A2A/#/documentation)
   - 🎥 觀看[示範影片](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **運行示例**
   - 📥 複製[官方倉庫](https://github.com/google/A2A)
   - 📝 按照 `/samples` 入面嘅說明操作

3. **構建自己嘅應用**
   - 🛠️ 使用官方庫或改編示例
   - 🏗️ 從基本 A2A 代理或客戶端開始


## 資源

### 官方文檔
- 🇺🇸 [技術文檔](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON 規範](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [Agent Card 規範](https://google.github.io/A2A/#/documentation?id=agent-card)

### 社區文檔
- 🇺🇸 [A2A TypeScript 指南](docs/a2a-typescript-guide.md) - 使用 TypeScript 實現 A2A 嘅全面指南
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - A2A 同 Model Context Protocol 嘅比較
- 🇺🇸 [理解 A2A 協議](docs/understanding-a2a-protocol.md) - 深入了解 A2A 協議概念
- 🇺🇸 [A2A 示例方法同 JSON 響應](docs/a2a-sample-methods-and-json-responses.md) - A2A 方法同響應嘅詳細示例
- 🇺🇸 [Python A2A](docs/python-a2a.md)：一個強大且易用嘅庫，用於實現 Google 嘅 [Agent-to-Agent (A2A) 協議](https://google.github.io/A2A/) - [連結](https://a2aprotocol.ai/blog/python-a2a)
- 🇨🇳 [A2A 協議介紹](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A 協議嘅中文介紹

## 論文

- 📄 [AI Agent 協議綜述](https://arxiv.org/pdf/2504.16736) - 一篇學術論文，調查了現有的 LLM agent 通信協議（包括 A2A 所屬的類別），對它們進行分類，分析性能，並討論未來挑戰。

[⬆️ 返回目錄](#contents)

## 實現方案

### 官方示例

#### Python
- 🐍 **通用庫**：核心 HTTP、JSON-RPC、SSE 處理 - [連結](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **主機（客戶端）**：命令行客戶端示例 - [連結](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **主機（代理）**：委派俾 A2A 代理嘅協調器代理 - [連結](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **伺服器庫**：核心伺服器實現 - [連結](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **客戶端庫**：客戶端實現 - [連結](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **主機（客戶端）**：命令行客戶端示例 - [連結](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

## 社區實現

| 名稱 | 作者 | 描述 | 星標 |
|------|--------|-------------|-------|
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | 專注於模塊化同可擴展性嘅 A2A 協議 TypeScript 實現 | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | 用於構建 A2A 伺服器嘅 Go 庫，附帶示例實現 | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | 遵循六角架構原則嘅地道 Rust 實現 | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | 用於 A2A 通訊嘅極簡 Python SDK | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A2A 協議嘅 C#/.NET 實現 | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | 用於將 A2A 協議集成到 NestJS 應用程序嘅模塊 | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | 用於實現 A2A 協議嘅易用 Python 庫 | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 用於托管、註冊、發現同與代理交互嘅 A2A 網絡實現 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | 基於 Google ADK 構建嘅 AI 代理開發框架，有助於為 A2A 網絡創建代理 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | 輕量級 A2A Python 實現 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A2A 嘅命令行客戶端 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A Test Suit](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A 測試套件 | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | 一個自託管的瀏覽器，使用內置MCP和A2A支持的代理 | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | 一個支援 MCP 的多智能體聊天應用，旨在通過 A2A 協議暴露智能體並作為客戶端連接到遠程 A2A 智能體 | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | 一個專注於開發者體驗和全面功能的 Agent2Agent 協議 JS/TS SDK | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |

[⬆️ 返回目錄](#contents)

### 框架整合

#### Python
- 🐍 **LangGraph**：貨幣轉換（功能：工具、流式處理、多輪會話）- [連結](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**：圖像生成（功能：非文本物件（文件））- [連結](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**：費用報銷（功能：多輪會話、表單（DataPart））- [連結](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**：用於實現 Google 嘅 [Agent-to-Agent (A2A) 協議](https://google.github.io/A2A/) 嘅強大且易用嘅庫 - [連結](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**：電影資訊/代碼生成（功能：工具、物件（文件）、非同步）- [連結](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### 社區示例

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**：帶有 A2A 伺服器同客戶端嘅編碼代理實現 - [連結](https://github.com/sing1ee/a2a-agent-coder)

[⬆️ 返回目錄](#contents)

## AgentCard

## 社區

- 🐛 [GitHub 議題](https://github.com/google/A2A/issues)
- 💬 [GitHub 討論](https://github.com/google/A2A/discussions/)

## 貢獻

歡迎貢獻！請先閱讀[貢獻指南](CONTRIBUTING.md)。
