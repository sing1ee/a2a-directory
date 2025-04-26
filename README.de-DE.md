# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## Inhaltsverzeichnis

- 📋 [Überblick](#überblick)
- 🚀 [Erste Schritte](#erste-schritte)
- 📚 [Ressourcen](#ressourcen)
- 💻 [Implementierungen](#implementierungen)
- 🎴 [AgentCard](#agentcard)
- 🤝 [Community-Implementierungen](#community-implementierungen)
- 👥 [Community](#community)
- 🤝 [Mitwirken](#mitwirken)


## Überblick

A2A (Agent2Agent) ist ein offenes Protokoll von Google, das KI-Agenten ermöglicht, sicher zu kommunizieren und zusammenzuarbeiten. Es bricht Silos zwischen isolierten Agentensystemen auf und ermöglicht komplexe anwendungsübergreifende Automatisierung.

**Hauptmerkmale:**
- 🎯 Einfach: Nutzt HTTP, JSON-RPC, SSE
- 🏢 Unternehmensbereit: Fokus auf Sicherheit und Datenschutz
- ⚡ Asynchron: Bewältigt langfristige Aufgaben
- 🔄 Modalitätsunabhängig: Unterstützt Text, Dateien, Formulare, Streams
- 🔒 Undurchsichtige Ausführung: Agenten interagieren ohne interne Logik zu teilen

**Offizielle Links:**
- 🌐 Website: [google.github.io/A2A](https://google.github.io/A2A)
- 📦 GitHub: [github.com/google/A2A](https://github.com/google/A2A)

## Erste Schritte

1. **Grundlagen lernen**
   - 📖 Lesen Sie die [technische Dokumentation](https://google.github.io/A2A/#/documentation)
   - 🎥 Schauen Sie das [Demo-Video an](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **Beispiele ausführen**
   - 📥 Klonen Sie das [offizielle Repository](https://github.com/google/A2A)
   - 📝 Folgen Sie den Anweisungen in `/samples`

3. **Eigene Entwicklung**
   - 🛠️ Verwenden Sie offizielle Bibliotheken oder passen Sie Beispiele an
   - 🏗️ Beginnen Sie mit einem einfachen A2A-Agenten oder -Client


## Ressourcen

### Offizielle Dokumentation
- 🇺🇸 [Technische Dokumentation](https://google.github.io/A2A/#/documentation)
- 🇺🇸 [JSON-Spezifikation](https://github.com/google/A2A/tree/main/specification/json)
- 🇺🇸 [Agent Card Spezifikation](https://google.github.io/A2A/#/documentation?id=agent-card)

### Community-Dokumentation
- 🇺🇸 [A2A TypeScript Leitfaden](docs/a2a-typescript-guide.md) - Ein umfassender Leitfaden zur Implementierung von A2A in TypeScript
- 🇺🇸 [A2A vs MCP](docs/a2a-vs-mcp.md) - Vergleich zwischen A2A und Model Context Protocol
- 🇺🇸 [Das A2A-Protokoll verstehen](docs/understanding-a2a-protocol.md) - Tieferer Einblick in die Konzepte des A2A-Protokolls
- 🇺🇸 [A2A Beispielmethoden und JSON-Antworten](docs/a2a-sample-methods-and-json-responses.md) - Detaillierte Beispiele für A2A-Methoden und Antworten
- 🇺🇸 [Python A2A](docs/python-a2a.md): Eine leistungsstarke und benutzerfreundliche Bibliothek zur Implementierung von Googles [Agent-to-Agent (A2A) Protokoll](https://google.github.io/A2A/) - [Link](https://a2aprotocol.ai/blog/python-a2a)
- 🇨🇳 [A2A Protokoll-Einführung](https://mp.weixin.qq.com/s/ySDTLuWvJeO9n7uBw2XxmQ) - Einführung zum A2A-Protokoll auf Chinesisch

## Wissenschaftliche Arbeiten

- 📄 [Eine Übersicht über KI-Agenten-Protokolle](https://arxiv.org/pdf/2504.16736) - Wissenschaftliche Arbeit, die bestehende LLM-Agenten-Kommunikationsprotokolle (einschließlich der Kategorie, zu der A2A gehört) untersucht, klassifiziert, die Leistung analysiert und zukünftige Herausforderungen diskutiert.

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## Implementierungen

### Offizielle Beispiele

#### Python
- 🐍 **Common Library**: Kern-HTTP, JSON-RPC, SSE-Handhabung - [Link](https://github.com/google/A2A/tree/main/samples/python/common)
- 🐍 **Host (Client)**: Kommandozeilen-Client-Beispiel - [Link](https://github.com/google/A2A/tree/main/samples/python/hosts/cli)
- 🐍 **Host (Agent)**: Orchestrator-Agent, der an A2A-Agenten delegiert - [Link](https://github.com/google/A2A/tree/main/samples/python/hosts/multiagent)

#### JavaScript/TypeScript
- 🚀 **Server Library**: Kern-Server-Implementierung - [Link](https://github.com/google/A2A/tree/main/samples/js/src/server)
- 🚀 **Client Library**: Client-Implementierung - [Link](https://github.com/google/A2A/tree/main/samples/js/src/client)
- 🚀 **Host (Client)**: Kommandozeilen-Client-Beispiel - [Link](https://github.com/google/A2A/blob/main/samples/js/src/cli.ts)

## Community-Implementierungen

| Name | Autor | Beschreibung | Sterne |
|------|--------|-------------|-------|
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | Eine TypeScript-Implementierung des A2A-Protokolls mit Fokus auf Modularität und Erweiterbarkeit | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [a2a-go](https://github.com/a2aserver/a2a-go) | [@a2aserver](https://github.com/a2aserver) | Eine Go-Bibliothek zum Erstellen von A2A-Servern mit Beispielimplementierungen | [![Stars](https://img.shields.io/github/stars/a2aserver/a2a-go?style=social)](https://github.com/a2aserver/a2a-go) |
| [a2a-rs](https://github.com/EmilLindfors/a2a-rs) | [@EmilLindfors](https://github.com/EmilLindfors) | Eine idiomatische Rust-Implementierung nach hexagonalen Architekturprinzipien | [![Stars](https://img.shields.io/github/stars/EmilLindfors/a2a-rs?style=social)](https://github.com/EmilLindfors/a2a-rs) |
| [a2a_min](https://github.com/pcingola/a2a_min) | [@pcingola](https://github.com/pcingola) | Ein minimalistisches Python-SDK für A2A-Kommunikation | [![Stars](https://img.shields.io/github/stars/pcingola/a2a_min?style=social)](https://github.com/pcingola/a2a_min) |
| [a2adotnet](https://github.com/azixaka/a2adotnet) | [@azixaka](https://github.com/azixaka) | Eine C#/.NET-Implementierung des A2A-Protokolls | [![Stars](https://img.shields.io/github/stars/azixaka/a2adotnet?style=social)](https://github.com/azixaka/a2adotnet) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | [@thestupd](https://github.com/thestupd) | Ein Modul zur Integration des A2A-Protokolls in NestJS-Anwendungen | [![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a?style=social)](https://github.com/thestupd/nestjs-a2a) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | [@themanojdesai](https://github.com/themanojdesai) | Eine benutzerfreundliche Python-Bibliothek zur Implementierung des A2A-Protokolls | [![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a?style=social)](https://github.com/themanojdesai/python-a2a) |
| [Aira](https://github.com/IhateCreatingUserNames2/Aira) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | Eine A2A-Netzwerkimplementierung zum Hosten, Registrieren, Entdecken und Interagieren mit Agenten | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Aira?style=social)](https://github.com/IhateCreatingUserNames2/Aira) |
| [Cognisphere](https://github.com/IhateCreatingUserNames2/Cognisphere) | [@IhateCreatingUserNames2](https://github.com/IhateCreatingUserNames2) | Ein KI-Agentenentwicklungsframework auf Basis von Googles ADK, das die Agentenerstellung potenziell für A2A-Netzwerke erleichtert | [![Stars](https://img.shields.io/github/stars/IhateCreatingUserNames2/Cognisphere?style=social)](https://github.com/IhateCreatingUserNames2/Cognisphere) |
| [a2a-server](https://github.com/chrishayuk/a2a-server) | [@chrishayuk](https://github.com/chrishayuk) | Eine leichtgewichtige A2A-Python-Implementierung | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-server?style=social)](https://github.com/chrishayuk/a2a-server) |
| [a2a-cli](https://github.com/chrishayuk/a2a-cli) | [@chrishayuk](https://github.com/chrishayuk) | Ein Kommandozeilen-Client für das A2A | [![Stars](https://img.shields.io/github/stars/chrishayuk/a2a-cli?style=social)](https://github.com/chrishayuk/a2a-cli) |
| [A2A Test-Suite](https://github.com/robert-at-pretension-io/A2A) | [@robert-at-pretension-io](https://github.com/robert-at-pretension-io) | A2A Test-Suite | [![Stars](https://img.shields.io/github/stars/robert-at-pretension-io/A2A?style=social)](https://github.com/robert-at-pretension-io/A2A) |
| [Grasp](https://github.com/aircodelabs/grasp) | [@adcentury](https://github.com/adcentury) | Ein selbstgehosteter Browser-Agent mit integrierter MCP- und A2A-Unterstützung | [![Stars](https://img.shields.io/github/stars/aircodelabs/grasp?style=social)](https://github.com/aircodelabs/grasp) |
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | Eine Multi-Agent-Chat-Anwendung mit MCP-Unterstützung, die darauf abzielt, Agenten über das A2A-Protokoll verfügbar zu machen und als Client mit entfernten A2A-Agenten zu verbinden | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

### Framework-Integrationen

#### Python
- 🐍 **LangGraph**: Währungsumrechnung (Funktionen: Tools, Streaming, Multi-Turn) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/langgraph)
- 🐍 **CrewAI**: Bilderzeugung (Funktionen: Nicht-textuelle Artefakte (Dateien)) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/crewai)
- 🐍 **Google ADK**: Spesenabrechnung (Funktionen: Multi-Turn, Formulare (DataPart)) - [Link](https://github.com/google/A2A/tree/main/samples/python/agents/google_adk)
- 🐍 **Python A2A**: Eine leistungsstarke und benutzerfreundliche Bibliothek zur Implementierung von Googles [Agent-to-Agent (A2A) Protokoll](https://google.github.io/A2A/) - [Link](https://github.com/themanojdesai/python-a2a)

#### JavaScript/TypeScript
- 🚀 **Genkit**: Filminformationen / Codegenerierung (Funktionen: Tools, Artefakte (Dateien), Asynchron) - [Link](https://github.com/google/A2A/tree/main/samples/js/src/agents)

### Community-Beispiele

#### JavaScript/TypeScript
- 🚀 **a2a-agent-coder**: Eine Coder-Agent-Implementierung mit A2A-Server und -Client - [Link](https://github.com/sing1ee/a2a-agent-coder)

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## AgentCard

## Community

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Diskussionen](https://github.com/google/A2A/discussions/)

## Mitwirken

Beiträge sind willkommen! Bitte lesen Sie zuerst die [Beitragsrichtlinien](CONTRIBUTING.md).