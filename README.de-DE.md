# ✨ A2A Directory ✨

![Awesome A2A](/images/a2a-directory.svg)

![PR Welcome](/images/prs-welcome.svg)

🌐 [English](README.md) | [中文](README.zh-CN.md) | [日本語](README.ja-JP.md) | [Deutsch](README.de-DE.md)

<a id="contents"></a>
## Inhaltsverzeichnis

- 📋 [Überblick](#überblick)
- 🚀 [Erste Schritte](#erste-schritte)
- 📚 [Ressourcen](#ressourcen)
- 🎯 [Offizielle Beispiele](#offizielle-beispiele)
- 🛠️ [Tools](#tools)
- 🤝 [Community-Implementierungen](#community-implementierungen)
- 🎨 [Community-Beispiele](#community-beispiele)
- 🔗 [Community-Links](#community-links)
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
- 📦 Offizielle Beispiele: [github.com/google/A2A-examples](https://github.com/google/A2A-examples)

## Erste Schritte

1. **Grundlagen lernen**
   - 📖 Lesen Sie die [technische Dokumentation](https://google.github.io/A2A/#/documentation)
   - 🎥 Schauen Sie das [Demo-Video an](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/A2A_demo_v4.mp4)

2. **Beispiele ausführen**
   - 📥 Klonen Sie das [offizielle Beispiel-Repository](https://github.com/google/A2A-examples)
   - 📝 Folgen Sie den Anweisungen für jedes Beispiel

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

## Offizielle Beispiele

### Python
- 🐍 **Basis-Agent**: Grundlegende A2A-Agenten-Implementierung - [Link](https://github.com/google/A2A-examples/tree/main/python/basic_agent)
- 🐍 **Host-Anwendung**: Host-Anwendung zur Interaktion mit A2A-Agenten - [Link](https://github.com/google/A2A-examples/tree/main/python/host_application)

### Go
- 🔷 **Basis-Agent**: A2A-Agenten-Implementierung in Go - [Link](https://github.com/google/A2A-examples/tree/main/go/basic_agent)
- 🔷 **Host-Anwendung**: Host-Anwendung in Go - [Link](https://github.com/google/A2A-examples/tree/main/go/host_application)

### JavaScript/TypeScript
- 🚀 **Basis-Agent**: A2A-Agenten-Implementierung in TypeScript - [Link](https://github.com/google/A2A-examples/tree/main/typescript/basic_agent)
- 🚀 **Host-Anwendung**: Host-Anwendung in TypeScript - [Link](https://github.com/google/A2A-examples/tree/main/typescript/host_application)

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## Tools

| Name | Autor | Beschreibung | Stars |
|------|--------|-------------|-------|
| [A2A-Protokoll-Validator](https://github.com/google/A2A-examples/tree/main/tools/validator) | [@google](https://github.com/google) | Validierungstool für A2A-Protokoll-Implementierungen | [![Stars](https://img.shields.io/github/stars/google/A2A-examples?style=social)](https://github.com/google/A2A-examples) |

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## Community-Implementierungen

| Name | Autor | Beschreibung | Stars |
|------|--------|-------------|-------|
| [a2a-python](https://github.com/google/a2a-python) | [@google](https://github.com/google) | Offizielles Python SDK für das Agent2Agent (A2A) Protokoll | [![Stars](https://img.shields.io/github/stars/google/a2a-python?style=social)](https://github.com/google/a2a-python) |
| [a2a-js](https://github.com/google-a2a/a2a-js) | [@google-a2a](https://github.com/google-a2a) | Offizielles JavaScript SDK für das Agent2Agent (A2A) Protokoll - Eine JavaScript-Bibliothek zur Ausführung agentischer Anwendungen als A2AServers | [![Stars](https://img.shields.io/github/stars/google-a2a/a2a-js?style=social)](https://github.com/google-a2a/a2a-js) |
| [a2ajava](https://github.com/vishalmysore/a2ajava) | [@vishalmysore](https://github.com/vishalmysore) | Eine reine Java-Implementierung des A2A-Protokolls für Spring Boot-Anwendungen mit Client- und Server-Implementierungen | [![Stars](https://img.shields.io/github/stars/vishalmysore/a2ajava?style=social)](https://github.com/vishalmysore/a2ajava) |
| [a2a4j](https://github.com/a2ap/a2a4j) | [@a2ap](https://github.com/a2ap) | A2A4J ist eine umfassende Java-Implementierung des Agent2Agent-Protokolls und stellt einen offenen Standard für die Kommunikation und Interoperabilität zwischen unabhängigen KI-Agentensystemen bereit. | [![Stars](https://img.shields.io/github/stars/a2ap/a2a4j?style=social)](https://github.com/a2ap/a2a4j) |
| [legion-a2a](https://github.com/TheRaLabs/legion-a2a) | [@TheRaLabs](https://github.com/TheRaLabs) | Eine TypeScript-Implementierung des A2A-Protokolls mit Fokus auf Modularität und Erweiterbarkeit | [![Stars](https://img.shields.io/github/stars/TheRaLabs/legion-a2a?style=social)](https://github.com/TheRaLabs/legion-a2a) |
| [trpc-a2a-go](https://github.com/trpc-group/trpc-a2a-go) | [@trpc-group](https://github.com/trpc-group) | Go A2A-Implementierung des tRPC-Teams mit vollständiger Client/Server-Unterstützung, In-Memory-Aufgabenverwaltung, Streaming-Antworten, Sitzungsverwaltung, mehreren Authentifizierungsmethoden (JWT, API-Schlüssel, OAuth2) und umfassenden Beispielen | [![Stars](https://img.shields.io/github/stars/trpc-group/trpc-a2a-go?style=social)](https://github.com/trpc-group/trpc-a2a-go) |
| [jira-a2a](https://github.com/tuannvm/jira-a2a) | [@tuannvm](https://github.com/tuannvm) | Das Jira A2A-System ist eine DevOps-Workflow-Automatisierungsplattform, die das tRPC-A2A-Go-Framework verwendet. Es besteht aus unabhängigen Go-Agents, die über A2A-Nachrichten miteinander kommunizieren. | [![Stars](https://img.shields.io/github/stars/tuannvm/jira-a2a?style=social)](https://github.com/tuannvm/jira-a2a) |
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
| [swissknife](https://github.com/daltonnyx/swissknife) | [@daltonnyx](https://github.com/daltonnyx) | Eine Multi-Agent-Chat-Anwendung mit MCP-Unterstützung, die darauf abzielt, Agenten über das A2A-Protokoll zu exponieren und als Client mit entfernten A2A-Agenten zu verbinden | [![Stars](https://img.shields.io/github/stars/daltonnyx/swissknife?style=social)](https://github.com/daltonnyx/swissknife) |
| [artinet-sdk](https://github.com/the-artinet-project/artinet-sdk) | [@the-artinet-project](https://github.com/the-artinet-project) | Ein JS/TS SDK für das Agent2Agent-Protokoll mit Fokus auf Entwicklererfahrung und umfassende Funktionen | [![Stars](https://img.shields.io/github/stars/the-artinet-project/artinet-sdk?style=social)](https://github.com/the-artinet-project/artinet-sdk) |
| [a2a-validation-tool](https://github.com/llmx-de/a2a-validation-tool) | [@llmx-de](https://github.com/llmx-de) | Eine Desktop-Anwendung zum Testen und Validieren von Agent-to-Agent (A2A) Protokoll-Implementierungen | [![Stars](https://img.shields.io/github/stars/llmx-de/a2a-validation-tool?style=social)](https://github.com/llmx-de/a2a-validation-tool) |
| [a2a-python-currency](https://github.com/sing1ee/a2a-python-currency) | [@sing1ee](https://github.com/sing1ee) | Eine Tutorial-Implementierung eines Währungs-Agenten mit dem A2A Python SDK | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-python-currency?style=social)](https://github.com/sing1ee/a2a-python-currency) |

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## Community-Beispiele

| Name | Autor | Beschreibung | Stars |
|------|--------|-------------|-------|
| [a2a-agent-coder](https://github.com/sing1ee/a2a-agent-coder) | [@sing1ee](https://github.com/sing1ee) | Eine Coder Agent-Implementierung mit A2A-Server und -Client | [![Stars](https://img.shields.io/github/stars/sing1ee/a2a-agent-coder?style=social)](https://github.com/sing1ee/a2a-agent-coder) |
| [agentic-trading](https://github.com/kweinmeister/agentic-trading) | [@kweinmeister](https://github.com/kweinmeister) | Eine Beispielanwendung zur Demonstration der Interoperabilität zwischen Google ADK und A2A für Handelsautomatisierung | [![Stars](https://img.shields.io/github/stars/kweinmeister/agentic-trading?style=social)](https://github.com/kweinmeister/agentic-trading) |
| [python-a2a-tutorial](https://github.com/sing1ee/python-a2a-tutorial) | [@sing1ee](https://github.com/sing1ee) | Ein umfassendes Tutorial zur A2A-Implementierung in Python mit praktischen Beispielen | [![Stars](https://img.shields.io/github/stars/sing1ee/python-a2a-tutorial?style=social)](https://github.com/sing1ee/python-a2a-tutorial) |
| [a2a-mcp-openrouter](https://github.com/Aamir-Mallick/a2a-mcp-openrouter) | [@Aamir-Mallick](https://github.com/Aamir-Mallick) | Ein Projekt, das A2A-Protokoll und MCP integriert und LLM-Zugang über OpenRouter bereitstellt | [![Stars](https://img.shields.io/github/stars/Aamir-Mallick/a2a-mcp-openrouter?style=social)](https://github.com/Aamir-Mallick/a2a-mcp-openrouter) |
| [a2a-mcp-bridge](https://github.com/Aamir-Mallick/a2a-mcp-bridge) | [@Aamir-Mallick](https://github.com/Aamir-Mallick) | Eine Brücken-Implementierung zwischen A2A-Protokoll und Model Context Protocol (MCP) | [![Stars](https://img.shields.io/github/stars/Aamir-Mallick/a2a-mcp-bridge?style=social)](https://github.com/Aamir-Mallick/a2a-mcp-bridge) |

[⬆️ Zurück zum Inhaltsverzeichnis](#contents)

## Community-Links

- 🐛 [GitHub Issues](https://github.com/google/A2A/issues)
- 💬 [GitHub Diskussionen](https://github.com/google/A2A/discussions/)

## Mitwirken

Beiträge sind willkommen! Bitte lesen Sie zuerst die [Beitragsrichtlinien](CONTRIBUTING.md).
