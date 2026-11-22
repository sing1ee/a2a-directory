# Contributing to A2A Directory

Thank you for your interest in contributing to the A2A Directory! This document provides guidelines and instructions for contributing to this project.

## How to Contribute

### 1. AgentCards

We welcome contributions of new AgentCards! When contributing an AgentCard:

- Follow the [Agent Card Specification](https://google.github.io/A2A/#/documentation?id=agent-card)
- Include clear documentation of the agent's capabilities
- Provide examples of usage
- Ensure compatibility with the A2A protocol

### 2. Community Documentation

Help us expand our documentation! You can contribute:

- Technical guides in any language
- Protocol comparisons and analyses
- Implementation tutorials
- Best practices and patterns

Current documentation language:
- 🇺🇸 English

### 3. Community Samples

Share your A2A implementations! We accept:

- Server implementations in any language
- Client implementations
- Framework integrations
- Example applications

Current supported languages:
- 🐍 Python
- 🚀 JavaScript/TypeScript
- 🦀 Rust
- 🐹 Go
- ☕ Java
- 💎 C#
- 🐘 PHP
- 🔵 Ruby
- 🦫 Swift
- 🦫 Kotlin

### 4. Reporting Issues

If you find a bug or have a feature request, please open an issue on GitHub. When reporting issues:

- Use a clear and descriptive title
- Provide detailed steps to reproduce the issue
- Include relevant code snippets or error messages
- Specify your environment (OS, Node.js version, etc.)

### 5. Submitting Pull Requests

We welcome pull requests! Here's how to submit one:

1. Star this repository on GitHub.
2. Fork the repository and create a branch for your changes.
3. Make your changes and submit a pull request.

GitHub Actions checks whether you have starred the repository when you open or reopen a pull request. If the check confirms you have not starred it, the pull request closes automatically. If the lookup fails, the pull request stays open. If the workflow closes your pull request, star the repository before asking a maintainer to reopen it.

Maintainers can set the `STARGAZERS_READ_TOKEN` Actions secret if the default workflow token cannot read the [stargazer list](https://docs.github.com/en/rest/activity/starring#list-stargazers). Use a fine-grained personal access token from a repository admin or collaborator, scoped to this repository with read access to Metadata. The repository's [Actions event policy](https://docs.github.com/en/actions/how-tos/administer/control-workflow-execution) must allow `pull_request_target`.

## Project Structure

The project is organized as follows:

- `docs/`: Documentation files
- `images/`: Image assets

## Development Setup

This is a documentation-only repository — no build step, dependencies, or tests are required.

1. Clone the repository
2. Make your changes to the relevant Markdown files
3. Submit a pull request

## Commit Message Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

Types:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `test`: Test-related changes
- `chore`: Maintenance tasks

## License

By contributing to this project, you agree that your contributions will be licensed under the project's license.

## Questions?

If you have any questions about contributing, please open an issue or contact the maintainers.
