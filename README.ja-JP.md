# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## 目次

- 📋 [概要](#overview)
- 🚀 [はじめに](#getting-started)
- 📚 [リソース](#resources)
- 🎯 [公式サンプル](#official-samples)
- 🛠️ [ツール](#tools)
- 🤝 [コミュニティ実装](#community-implementations)
- 🎨 [コミュニティサンプル](#community-samples)
- 🔗 [コミュニティリンク](#community-links)
- 🤝 [貢献](#contributing)


## 概要

A2A（Agent2Agent）はGoogleが提供するオープンプロトコルで、AIエージェントが安全に通信し協力することを可能にします。孤立したエージェントシステム間の障壁を取り除き、複雑なクロスアプリケーション自動化を実現します。

**主な特徴:**
- 🎯 シンプル：HTTP、JSON-RPC、SSEを使用
- 🏢 エンタープライズ対応：セキュリティとプライバシーに焦点
- ⚡ 非同期優先：長時間実行タスクを処理
- 🔄 モダリティに依存しない：テキスト、ファイル、フォーム、ストリームをサポート
- 🔒 不透明な実行：エージェントは内部ロジックを共有せずに相互作用

**公式リンク:**
- 🌐 ウェブサイト: [google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub: [github.com/google/A2A](https://github.com/google/A2A)
- 📦 公式サンプル: [github.com/google/A2A-examples](https://github.com/google/A2A-examples)

## はじめに

1. **基本を学ぶ**
   - 📖 [技術ドキュメント](https://google.github.io/A2A/#/documentation)を読む
   - 🎥 [デモビデオ](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)を見る

2. **サンプルを実行する**
   - 📥 [公式サンプルリポジトリ](https://github.com/google/A2A-examples)をクローン
   - 📝 各サンプルの指示に従う

3. **独自のものを構築する**
   - 🛠️ 公式ライブラリを使用するか、サンプルを適応させる
   - 🏗️ 基本的なA2Aエージェントまたはクライアントから始める


## リソース

### 公式ドキュメント
- 🇺🇸 [技術ドキュメント](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON仕様](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [エージェントカード仕様](https://google.github.io/A2A/#/documentation?id=agent-card)

### コミュニティドキュメント
- 🇺🇸 [A2A TypeScriptガイド](docs/a2a-typescript-guide.md) - TypeScriptでA2Aを実装するための包括的なガイド
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - A2AとModel Context Protocolの比較
- 🇺🇸 [A2Aプロトコルの理解](docs/understanding-a2a-protocol.md) - A2Aプロトコルの概念を深く掘り下げる
- 🇺🇸 [A2AサンプルメソッドとJSON応答](docs/a2a-sample-methods-and-json-responses.md) - A2Aメソッドと応答の詳細な例
- 🇺🇸 [Python A2A](docs/python-a2a.md): Google の [Agent-to-Agent (A2A) プロトコル](https://google.github.io/A2A/) を実装するための強力で使いやすいライブラリ - [リンク](https://a2aprotocol.ai/blog/python-a2a)
- 🇨🇳 [A2A プロトコル紹介](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A プロトコルの中国語紹介

## 論文

- 📄 [AI Agent プロトコルの調査](https://arxiv.org/pdf/2504.16736) - 既存の LLM agent 通信プロトコル（A2A が属するカテゴリを含む）を調査し、分類し、性能を分析し、将来の課題について議論する学術論文。

[⬆️ 目次に戻る](#contents)

## 公式サンプル

### Python
- 🐍 **基本エージェント**: 基本的なA2Aエージェント実装 - [リンク](https://github.com/google/A2A-examples/tree/main/python/basic_agent)
- 🐍 **ホストアプリケーション**: A2Aエージェントと対話するホストアプリケーション - [リンク](https://github.com/google/A2A-examples/tree/main/python/host_application)

### Go
- 🔷 **基本エージェント**: Go言語でのA2Aエージェント実装 - [リンク](https://github.com/google/A2A-examples/tree/main/go/basic_agent)
- 🔷 **ホストアプリケーション**: Go言語でのホストアプリケーション - [リンク](https://github.com/google/A2A-examples/tree/main/go/host_application)

### JavaScript/TypeScript
- 🚀 **基本エージェント**: TypeScriptでのA2Aエージェント実装 - [リンク](https://github.com/google/A2A-examples/tree/main/typescript/basic_agent)
- 🚀 **ホストアプリケーション**: TypeScriptでのホストアプリケーション - [リンク](https://github.com/google/A2A-examples/tree/main/typescript/host_application)

[⬆️ 目次に戻る](#contents)

## ツール

| 名前 | 作者 | 説明 | Stars |
|------|--------|-------------|-------|
| [A2Aプロトコルバリデーター](https://github.com/google/A2A-examples/tree/main/tools/validator) | [@google](https://github.com/google) | A2Aプロトコル実装の検証ツール | [![Stars](https://img.shields.io/github/stars/google/A2A-examples?style=social)](https://github.com/google/A2A-examples) |

[⬆️ 目次に戻る](#contents)

## コミュニティ実装

| 名前 | 作者 | 説明 | Stars |
|------|--------|-------------|-------|
| [a2a-python](https://github.com/google/a2a-python) | [@google](https://github.com/google) | Google 公式の Agent2Agent (A2A) プロトコル Python SDK | [![Stars](https://img.shields.io/github/stars/google/a2a-python?style=social)](https://github.com/google/a2a-python) |
| [a2ajava](https://github.com/vishalmysore/a2ajava) | [@vishalmysore](https://github.com/vishalmysore) | Spring Boot アプリケーション向けの純粋な Java 実装の A2A プロトコル、クライアントとサーバーの両方の実装を含む | [![Stars](https://img.shields.io/github/stars/vishalmysore/a2ajava?style=social)](https://github.com/vishalmysore/a2ajava) |
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | モジュール性と拡張性に焦点を当てた TypeScript による A2A プロトコル実装 | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [trpc-a2a-go](https://github.com/trpc-group/trpc-a2a-go) | [@trpc-group](https://github.com/trpc-group) | tRPCチームによるGo A2A実装。完全なクライアント/サーバーサポート、インメモリタスク管理、ストリーミングレスポンス、セッション管理、複数の認証方法（JWT、APIキー、OAuth2）、包括的な例を提供 | [![Stars](https://img.shields.io/github/stars/trpc-group/trpc-a2a-go?style=social)](https://github.com/trpc-group/trpc-a2a-go) |
| [jira-a2a](https://github.com/tuannvm/jira-a2a) | [@tuannvm](https://github.com/tuannvm) | Jira A2A システムは、tRPC-A2A-Go フレームワークを使用した DevOps ワークフロー自動化プラットフォームです。これは、A2A メッセージを介して通信する独立した Go エージェントで構成されています。 | [![Stars](https://img.shields.io/github/stars/tuannvm/jira-a2a?style=social)](https://github.com/tuannvm/jira-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | A2Aサーバーを構築するためのGoライブラリ（実装例付き） | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | ヘキサゴナルアーキテクチャの原則に従った慣用的なRust実装 | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | A2A通信のためのミニマリスティックなPython SDK | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | A2AプロトコルのC#/.NET実装 | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | A2AプロトコルをNestJSアプリケーションに統合するためのモジュール | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | A2Aプロトコルを実装するための使いやすいPythonライブラリ | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | エージェントのホスティング、登録、発見、相互作用のためのA2Aネットワーク実装 | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | GoogleのADK上に構築されたAIエージェント開発フレームワーク（A2Aネットワーク向けエージェント作成を促進） | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | 軽量なA2A Pythonの実装 | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | A2Aのためのコマンドラインクライアント | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A テストスイート](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A テストスイート | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | MCPとA2Aサポートを内蔵したセルフホスト型ブラウザエージェント | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | MCPをサポートするマルチエージェントチャットアプリケーションで、A2Aプロトコルを通じてエージェントを公開し、クライアントとしてリモートA2Aエージェントに接続することを目的としています | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | 開発者体験と包括的な機能に焦点を当てたAgent2AgentプロトコルのJS/TS SDK | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |
| [a2a-validation-tool](https://github.com/llmx-de/a2a-validation-tool) | [@llmx-de](https://github.com/llmx-de) | Agent-to-Agent (A2A) プロトコル実装のテストと検証のためのデスクトップアプリケーション | [![Stars](https://img.shields.io/github/stars/llmx-de/a2a-validation-tool?style=social)](https://github.com/llmx-de/a2a-validation-tool) |
| [a2a-python-currency](https://github.com/sing1ee/a2a-python-currency) | [@sing1ee](https://github.com/sing1ee) | A2A Python SDKを使用した通貨エージェントのチュートリアル実装 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-python-currency?style=social)](https://github.com/sing1ee/a2a-python-currency) |

[⬆️ 目次に戻る](#contents)

[⬆️ 目次に戻る](#contents)

## コミュニティサンプル

| 名前 | 作者 | 説明 | Stars |
|------|--------|-------------|-------|
| [a2a-agent-coder](https://github.com/sing1ee/a2a-agent-coder) | [@sing1ee](https://github.com/sing1ee) | A2Aサーバーとクライアントを備えたCoder Agentの実装 | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-agent-coder?style=social)](https://github.com/sing1ee/a2a-agent-coder) |
| [agentic-trading](https://github.com/kweinmeister/agentic-trading) | [@kweinmeister](https://github.com/kweinmeister) | Google ADKとA2Aの相互運用性を示す取引自動化のサンプルアプリケーション | [![Stars](https://img.shields.io/github/stars/kweinmeister/agentic-trading?style=social)](https://github.com/kweinmeister/agentic-trading) |
| [python-a2a-tutorial](https://github.com/sing1ee/python-a2a-tutorial) | [@sing1ee](https://github.com/sing1ee) | 実践的な例を含むPython A2A実装の包括的なチュートリアル | [![Stars](https://img.shields.io/github/stars/sing1ee/python-a2a-tutorial?style=social)](https://github.com/sing1ee/python-a2a-tutorial) |
| [a2a-mcp-openrouter](https://github.com/Aamir-Mallick/a2a-mcp-openrouter) | [@Aamir-Mallick](https://github.com/Aamir-Mallick) | A2AプロトコルとMCPを統合し、OpenRouterを通じてLLMアクセスを提供するプロジェクト | [![Stars](https://img.shields.io/github/stars/Aamir-Mallick/a2a-mcp-openrouter?style=social)](https://github.com/Aamir-Mallick/a2a-mcp-openrouter) |
| [a2a-mcp-bridge](https://github.com/Aamir-Mallick/a2a-mcp-bridge) | [@Aamir-Mallick](https://github.com/Aamir-Mallick) | A2AプロトコルとModel Context Protocol (MCP)間のブリッジ実装 | [![Stars](https://img.shields.io/github/stars/Aamir-Mallick/a2a-mcp-bridge?style=social)](https://github.com/Aamir-Mallick/a2a-mcp-bridge) |

[⬆️ 目次に戻る](#contents)

## コミュニティリンク

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## 貢献

貢献は歓迎します！まずは[貢献ガイドライン](CONTRIBUTING.md)をお読みください。