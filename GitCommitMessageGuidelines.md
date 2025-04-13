# Git Commit Message Guidelines

## Commit Message Format

Each commit message consists of a **header**, a **body**, and a **footer**. The header has a special format that includes a **type**, a **scope**, and a **subject**:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and the **scope** of the header is optional.

Any line of the commit message cannot be longer than 100 characters. This allows the message to be easier to read on GitHub as well as in various git tools.

## Type

Must be one of the following:

* **feat**: A new feature
* **fix**: A bug fix
* **docs**: Documentation only changes
* **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **refactor**: A code change that neither fixes a bug nor adds a feature
* **perf**: A code change that improves performance
* **test**: Adding missing tests or correcting existing tests
* **build**: Changes that affect the build system or external dependencies
* **ci**: Changes to our CI configuration files and scripts
* **chore**: Other changes that don't modify src or test files
* **revert**: Reverts a previous commit

## Scope

The scope should be the name of the module affected (as perceived by the person reading the changelog generated from commit messages).

## Subject

The subject contains a succinct description of the change:

* Use the imperative, present tense: "change" not "changed" nor "changes"
* Don't capitalize the first letter
* No dot (.) at the end

## Body

The body should include the motivation for the change and contrast this with previous behavior.

## Footer

The footer should contain any information about **Breaking Changes** and is also the place to reference GitHub issues that this commit **Closes**.

Breaking Changes should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

## Examples

```
feat(auth): add login functionality

Implement JWT-based authentication system with login and logout capabilities.

Closes #123
```

```
fix(dashboard): resolve data loading issue

The dashboard was not loading data correctly due to an API endpoint mismatch.
This commit updates the endpoint URL and adds error handling.

Fixes #456
```

```
docs(readme): update installation instructions

Update the README with more detailed installation steps and troubleshooting tips.
```

```
style(users): format code according to style guide

No functional changes, just formatting.
```

```
refactor(api): simplify request handling logic

Simplified the request processing pipeline to make it more maintainable.
No functional changes or bug fixes included.
```

```
BREAKING CHANGE: change authentication API

The authentication API now requires a token parameter instead of using cookies.
Users will need to update their client implementations.

Migration guide: https://example.com/migration
```