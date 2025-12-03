# Contributing to CogniDigest-AI-Web-Content-Summarizer-Browser-Extension

We are thrilled you're considering contributing to **CogniDigest-AI-Web-Content-Summarizer-Browser-Extension**! Your efforts help us build a more powerful and intelligent web summarization tool. This document outlines the guidelines and best practices for contributing to this project.

## Code of Conduct

Please note that this project is released with a Contributor Code of Conduct. By participating in this project, you agree to abide by its terms. We expect all contributors to adhere to our [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md).

## How Can I Contribute?

There are many ways to contribute, not just by writing code.

### ‍🐛 Reporting Bugs

A good bug report is invaluable. Before opening a new issue, please:

1.  **Search Existing Issues**: Check if the bug has already been reported.
2.  **Verify**: Try to reproduce the bug on the latest `main` branch.
3.  **Open a New Issue**: If it's a new bug, please use our [bug report template](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/issues/new?assignees=&labels=bug&projects=&template=bug_report.md&title=%5BBug%5D+).
    *   Clearly describe the bug, including steps to reproduce.
    *   Provide screenshots or recordings if applicable.
    *   Specify your browser version, OS, and any relevant extension details.

### ✨ Suggesting Enhancements

We welcome ideas for new features or improvements!

1.  **Search Existing Issues/Discussions**: See if your idea has already been proposed.
2.  **Open a New Issue**: Use a general issue or discussion to describe your suggestion.
    *   Clearly articulate the problem your suggestion solves.
    *   Explain how your enhancement would work and its benefits.
    *   Provide mockups or examples if possible.

### 💻 Your First Code Contribution

New to open source? Start with issues labeled [`good first issue`](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/labels/good%20first%20issue). These are typically smaller, isolated tasks suitable for new contributors.

### 🚀 Pull Request Process

1.  **Fork the Repository**: Start by forking `https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension` to your GitHub account.
2.  **Clone Your Fork**:
    bash
    git clone https://github.com/YOUR_USERNAME/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension.git
    cd CogniDigest-AI-Web-Content-Summarizer-Browser-Extension
    
3.  **Create a New Branch**:
    bash
    git checkout -b feature/my-awesome-feature-name main
    
    *   Branch names should be descriptive (e.g., `feature/add-summarize-button`, `fix/login-bug`).
4.  **Make Your Changes**: Implement your feature or bug fix.
5.  **Run Tests & Linting**: Ensure your changes don't introduce regressions and adhere to coding standards.
    bash
    pnpm install # or npm install / yarn install if you prefer
    pnpm test
    pnpm biome check --apply-unsafe .
    pnpm biome format --write .
    
6.  **Commit Your Changes**: Follow the [Conventional Commits specification](#conventional-commits).
    bash
    git add .
    git commit -m "feat: add instant summarization button"
    
7.  **Push to Your Fork**:
    bash
    git push origin feature/my-awesome-feature-name
    
8.  **Open a Pull Request (PR)**:
    *   Go to your fork on GitHub and open a new PR against the `main` branch of the original repository.
    *   Please use our [pull request template](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/compare/main...chirag127:CogniDigest-AI-Web-Content-Summarizer-Browser-Extension:main?expand=1&template=pull_request_template.md).
    *   Provide a clear title and description of your changes.
    *   Link any relevant issues (e.g., `Closes #123`).
    *   Ensure all CI checks pass.

## Development Setup

### Prerequisites

*   **Node.js**: LTS version (e.g., v20.x or higher). We recommend using `pnpm` for package management.
*   **Web Browser**: Chrome (preferred for Manifest V3 development), Edge, or Firefox.

### Installation

1.  **Clone the Repository**:
    bash
    git clone https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension.git
    cd CogniDigest-AI-Web-Content-Summarizer-Browser-Extension
    
2.  **Install Dependencies**:
    bash
    pnpm install
    

### Running the Development Server

The project uses Vite and WXT for browser extension development.

bash
pnpm dev

This will start a development server and watch for changes.

### Building the Extension for Production

bash
pnpm build

This command compiles the extension into the `dist/` directory, ready for deployment.

### Loading the Extension in Your Browser (Manifest V3)

1.  Open your browser (e.g., Chrome).
2.  Navigate to `chrome://extensions` (or `edge://extensions`, `about:debugging#/runtime/this-firefox` for Firefox).
3.  Enable "Developer mode" (usually a toggle in the top right).
4.  Click "Load unpacked".
5.  Select the `dist/` directory from your cloned repository.
6.  The `CogniDigest AI` extension should now appear in your browser.

### Running Tests

We use `Vitest` for unit tests and `Playwright` for end-to-end (E2E) tests.

*   **Unit Tests**:
    bash
    pnpm test # Runs all Vitest tests
    
*   **End-to-End Tests**:
    bash
    pnpm test:e2e # Runs Playwright tests
    

### Linting and Formatting

We use `Biome` for code linting and formatting to maintain consistent code style.

*   **Check for Issues**:
    bash
    pnpm biome check .
    
*   **Apply Fixes (safe)**:
    bash
    pnpm biome check --apply .
    
*   **Apply Fixes (unsafe - use with caution)**:
    bash
    pnpm biome check --apply-unsafe .
    
*   **Format Code**:
    bash
    pnpm biome format --write .
    

## Coding Guidelines

### 🎨 Style Guide

*   We adhere to the code style enforced by `Biome`. Please ensure your code passes all `biome check` and `biome format` commands.
*   Follow best practices for TypeScript, including strict typing, clear interfaces, and modular components.
*   Prioritize readability, maintainability, and performance in your code.

### 📝 Conventional Commits

We use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit messages. This helps us generate changelogs and understand the history more easily.

**Examples:**
*   `feat: add instant summarization to context menu`
*   `fix: resolve UI layout shift on popup open`
*   `docs: update contributing guidelines`
*   `chore: update vite and wxt dependencies`
*   `refactor: restructure LLM integration module`

### 🌿 Branching Model

*   All new features and bug fixes should be developed on dedicated branches forked from `main`.
*   Direct commits to `main` are strictly forbidden.
*   Ensure your branch is rebased on the latest `main` before opening a PR to minimize merge conflicts.

## Security Vulnerabilities

If you discover a security vulnerability, please report it responsibly. Refer to our [Security Policy](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/.github/SECURITY.md) for details on how to report vulnerabilities.

## License

By contributing to CogniDigest-AI-Web-Content-Summarizer-Browser-Extension, you agree that your contributions will be licensed under its [CC BY-NC 4.0 License](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/LICENSE).

Thank you for your valuable contribution!
