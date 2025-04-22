# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## 目次

- 📋 [概要](#overview)
- 🚀 [はじめに](#getting-started)
- 📚 [リソース](#resources)
- 💻 [実装](#implementations)
- 🎴 [AgentCard](#agentcard)
- 🤝 [コミュニティ実装](#community-implementations)
- 👥 [コミュニティ](#community)
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

## はじめに

1. **基本を学ぶ**
   - 📖 [技術ドキュメント](https://google.github.io/A2A/#/documentation)を読む
   - 🎥 [デモビデオ](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)を見る

2. **サンプルを実行する**
   - 📥 [公式リポジトリ](https://github.com/google/A2A)をクローン
   - 📝 `/samples`の指示に従う

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

[⬆️ 目次に戻る](#contents)

## 実装

### 公式サンプル

#### Python
- 🐍 **共通ライブラリ**: コアHTTP、JSON-RPC、SSE処理 - [リンク](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **ホスト（クライアント）**: コマンドラインクライアント例 - [リンク](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **ホスト（エージェント）**: A2Aエージェントに委任するオーケストレーターエージェント - [リンク](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **サーバーライブラリ**: コアサーバー実装 - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **クライアントライブラリ**: クライアント実装 - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **ホスト（クライアント）**: コマンドラインクライアント例 - [リンク](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

## コミュニティ実装

| 名前 | 作者 | 説明 | スター |
|------|--------|-------------|-------|
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | モジュール性と拡張性に焦点を当てたA2Aプロトコルのタイプスクリプト実装 | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
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

[⬆️ 目次に戻る](#contents)

### フレームワーク統合

#### Python
- 🐍 **LangGraph**: 通貨変換（機能：ツール、ストリーミング、マルチターン） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**: 画像生成（機能：非テキストアーティファクト（ファイル）） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**: 経費精算（機能：マルチターン、フォーム（DataPart）） - [リンク](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**: Googleの[Agent-to-Agent (A2A) プロトコル](https://google.github.io/A2A/)を実装するための強力で使いやすいライブラリ - [リンク](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**: 映画情報/コード生成（機能：ツール、アーティファクト（ファイル）、非同期） - [リンク](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### コミュニティサンプル

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**: A2Aサーバーとクライアントを備えたCoderエージェント実装 - [リンク](https://github.com/sing1ee/a2a-agent-coder)

[⬆️ 目次に戻る](#contents)

## AgentCard

## コミュニティ

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Discussions](https://github.com/google/A2A/discussions/)

## 貢献

貢献は歓迎します！まずは[貢献ガイドライン](CONTRIBUTING.md)をお読みください。