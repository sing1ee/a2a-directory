# ✨ Agent2Agent プロトコル ✨

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md)

## 目次

- 📋 [概要](#概要)
- 🚀 [はじめに](#はじめに)
- 📚 [リソース](#リソース)
- 💻 [実装](#実装)
- 🎴 [AgentCard](#agentcard)
- 👥 [コミュニティ](#コミュニティ)
- 🤝 [貢献](#貢献)

## 概要

A2A (Agent2Agent) は、Google が提供するオープンプロトコルで、AI エージェントが安全に通信し、協力し合うことを可能にします。孤立したエージェントシステム間の壁を打破し、複雑なクロスアプリケーション自動化を実現します。

**主な特徴：**
- 🎯 シンプル：HTTP、JSON-RPC、SSE を使用
- 🏢 エンタープライズ対応：セキュリティとプライバシーに重点
- ⚡ 非同期優先：長時間実行タスクの処理
- 🔄 モダリティ非依存：テキスト、ファイル、フォーム、ストリームをサポート
- 🔒 不透明な実行：エージェントは内部ロジックを共有せずに相互作用

**公式リンク：**
- 🌐 ウェブサイト：[google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub：[github.com/google/A2A](https://github.com/google/A2A)

## はじめに

1. **基本を学ぶ**
   - 📖 [技術文書](https://google.github.io/A2A/#/documentation)を読む
   - 🎥 [デモ動画](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)を視聴

2. **サンプルを実行**
   - 📥 [公式リポジトリ](https://github.com/google/A2A)をクローン
   - 📝 `/samples` ディレクトリの指示に従う

3. **独自の実装を構築**
   - 🛠️ 公式ライブラリを使用するか、サンプルを改変
   - 🏗️ 基本的な A2A エージェントまたはクライアントから始める

## リソース

### 公式ドキュメント
- 🇺🇸 [技術文書](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON 仕様](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [エージェントカード仕様](https://google.github.io/A2A/#/documentation?id=agent-card)

### コミュニティドキュメント
- 🇺🇸 [A2A TypeScript ガイド](docs/a2a-typescript-guide.md) - TypeScript での A2A 実装の包括的ガイド
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - A2A とモデルコンテキストプロトコルの比較
- 🇺🇸 [A2A プロトコルの理解](docs/understanding-a2a-protocol.md) - A2A プロトコル概念の詳細な解説
- 🇺🇸 [A2A サンプルメソッドと JSON レスポンス](docs/a2a-sample-methods-and-json-responses.md) - A2A メソッドとレスポンスの詳細な例
- 🇺🇸 [Python A2A：Google Agent-to-Agent プロトコル完全ガイド](docs/python-a2a.md) - Python A2A は、Google の [Agent-to-Agent (A2A) プロトコル](https://google.github.io/A2A/) を実装するための強力で使いやすいライブラリです
- 🇨🇳 [A2A プロトコル紹介](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - A2A プロトコルの中国語紹介

## 実装

### 公式サンプル

#### Python
- 🐍 **共通ライブラリ**：コア HTTP、JSON-RPC、SSE 処理 - [リンク](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **ホスト（クライアント）**：コマンドラインクライアント例 - [リンク](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **ホスト（エージェント）**：複数の A2A エージェントを調整するオーケストレーター - [リンク](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **サーバーライブラリ**：コアサーバー実装 - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **クライアントライブラリ**：クライアント実装 - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **ホスト（クライアント）**：コマンドラインクライアント例 - [リンク](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

### フレームワーク統合

#### Python
- 🐍 **LangGraph**：通貨変換（機能：ツール、ストリーミング、マルチターン） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**：画像生成（機能：非テキストアーティファクト（ファイル）） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**：経費精算（機能：マルチターン、フォーム（DataPart）） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**：Google の [Agent-to-Agent (A2A) プロトコル](https://google.github.io/A2A/) を実装するための強力で使いやすいライブラリ - [リンク](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**：映画情報/コード生成（機能：ツール、アーティファクト（ファイル）、非同期） - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### コミュニティサンプル

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**：A2A サーバーとクライアントを備えたコーダーエージェント実装 - [リンク](https://github.com/sing1ee/a2a-agent-coder)

## AgentCard

## コミュニティ

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## 貢献

貢献をお待ちしています！まず[貢献ガイドライン](CONTRIBUTING.md)をお読みください。 