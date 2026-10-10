# Contributing Guidelines

Thank you for your interest in contributing to this project! By participating, you agree to follow these guidelines to ensure a smooth and collaborative development process.

---

## Table of Contents

- [Getting Started](#getting-started)
- [Code Style](#code-style)
- [Commit Messages](#commit-messages)
- [Branching & Pull Requests](#branching--pull-requests)
- [Testing](#testing)
- [Reporting Issues](#reporting-issues)
- [License](#license)

---

## Getting Started

1. **Fork the repository** and clone your fork locally.
   ```bash
   git clone https://github.com/<your-username>/repo-name.git
   cd repo-name
   ```
2. **Create a new branch** for your work:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Install dependencies** (if applicable):
   ```bash
   # Example for Python projects
   pip install -r requirements.txt
   ```
4. Ensure the test suite passes before you start:
   ```bash
   # Example for pytest
   pytest
   ```

---

## Code Style

- Follow the existing coding conventions used throughout the codebase.
- Use [PEP 8](https://peps.python.org/pep-0008/) for Python files, or the appropriate style guide for other languages.
- Run the linter before committing:
  ```bash
  # Example for flake8
  flake8 .
  ```
- Keep line length to **80 characters** where possible.
- Use meaningful variable and function names; avoid abbreviations unless they are widely understood.

---

## Commit Messages

Write clear, concise commit messages using the following format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

- **type** – one of `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.
- **scope** – optional, the part of the codebase affected (e.g., `parser`, `ui`).
- **subject** – short description (max 50 characters).
- **body** – optional, longer description of what and why.
- **footer** – optional, references to issues (e.g., `Closes #123`).

Example:
```
feat(parser): add support for nested expressions

Implemented recursive descent parsing for nested arithmetic expressions.
Closes #42
```

---

## Branching & Pull Requests

1. **Branch Naming** – Use `type/short-description` (e.g., `feat/add-login`).
2. **Pull Request (PR) Title** – Should be a concise summary of the change, prefixed with the same type used in commits (e.g., `feat: add login flow`).
3. **PR Description** – Include:
   - A brief overview of the change.
   - Motivation and related issue numbers.
   - Any breaking changes.
4. **Review Process** – At least one other maintainer must approve the PR before it can be merged.
5. **Rebase & Squash** – Keep a linear history. Rebase your branch onto the latest `main` and squash commits into logical units before merging.

---

## Testing

- Add tests for new functionality and ensure existing tests continue to pass.
- Follow the project's testing conventions (e.g., `pytest` for Python).
- Run the full test suite locally before submitting a PR:
  ```bash
  pytest
  ```

---

## Reporting Issues

- Use the GitHub Issues tracker.
- Provide a clear title, description, steps to reproduce, expected vs. actual behavior, and any relevant logs or screenshots.
- Tag the issue with appropriate labels (bug, enhancement, documentation, etc.).

---

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (see `LICENSE`).

---

Thank you for helping improve this project! 🎉
