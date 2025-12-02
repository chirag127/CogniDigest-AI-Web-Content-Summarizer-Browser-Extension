# Contributing to ContextLens-AI-Powered-Web-Summarizer-Browser-Extension

Thank you for your interest in contributing to `ContextLens-AI-Powered-Web-Summarizer-Browser-Extension`! We aim to build a high-quality, production-ready browser extension that adheres to the highest industry standards. Your contributions are invaluable in helping us achieve this goal.

## 1. Our Guiding Principles

As outlined in the `AGENTS.md` file, all contributions are expected to align with the **Apex Technical Authority** philosophy: "Zero-Defect, High-Velocity, Future-Proof."

This means prioritizing:

*   **Code Quality:** Clean, well-documented, and maintainable code.
*   **Performance:** Efficient and responsive user experience.
*   **Security:** Robust protection against vulnerabilities.
*   **Maintainability:** Adherence to architectural patterns and best practices.
*   **Professionalism:** Maintaining a high standard in all aspects of development and documentation.

## 2. Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

*   **Node.js:** Version 18.x or later (ensure compatibility with `manifest-v3`).
*   **npm:** Bundled with Node.js.
*   **Git:** For version control.
*   **Browser:** Chrome or Firefox for testing.

### Development Environment Setup

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/ContextLens-AI-Powered-Web-Summarizer-Browser-Extension.git
    cd ContextLens-AI-Powered-Web-Summarizer-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    

3.  **Build the Extension (Development Mode):**
    The project uses `vite` for building. Development builds will typically watch for changes and enable hot-reloading where applicable.
    bash
    npm run dev
    

4.  **Load the Extension in your Browser:**
    *   **Chrome:** Navigate to `chrome://extensions/`, enable 'Developer mode', click 'Load unpacked', and select the `dist` (or similar build output) directory.
    *   **Firefox:** Navigate to `about:debugging#/runtime/this-firefox`, click 'Load Temporary Add-on', and select the `manifest.json` file from the project root.

## 3. Contribution Workflow

We follow a standard GitHub pull request workflow:

1.  **Fork the Repository:** Create your own fork of the `chirag127/ContextLens-AI-Powered-Web-Summarizer-Browser-Extension` repository.
2.  **Create a Branch:** Create a new branch for your feature or bug fix:
    bash
    git checkout -b my-feature-branch
    
    *(Use descriptive branch names like `feat/add-new-summary-model` or `fix/incorrect-api-key-handling`.)*
3.  **Make Your Changes:** Implement your changes, ensuring they adhere to the project's coding standards and architectural guidelines.
4.  **Test Your Changes:** Run the relevant tests to ensure your changes haven't introduced regressions.
    bash
    npm test
    
    *(Add new tests for any new functionality or bug fixes.)*
5.  **Lint and Format:** Ensure your code is clean and formatted correctly.
    bash
    npm run lint
    npm run format
    
6.  **Commit Your Changes:** Write clear, concise commit messages.
    bash
    git add .
    git commit -m "feat: Add support for summarization history"
    
7.  **Push to Your Fork:**
    bash
    git push origin my-feature-branch
    
8.  **Open a Pull Request:** Submit a pull request from your fork's `my-feature-branch` to the `main` branch of the `chirag127/ContextLens-AI-Powered-Web-Summarizer-Browser-Extension` repository.

## 4. Code Standards & Best Practices

*   **TypeScript:** Use TypeScript with strict type checking enabled.
*   **Linting & Formatting:** Adhere to the linting and formatting rules enforced by Biome (as per Apex standards for modern JS/TS projects).
*   **Testing:** Write comprehensive unit and integration tests using Vitest. End-to-end tests using Playwright should be considered for critical user flows.
*   **Architecture:** Follow the Feature-Sliced Design (FSD) principles where applicable, promoting modularity and separation of concerns.
*   **`manifest-v3`:** Ensure all changes comply with Chrome's Manifest V3 guidelines.
*   **AI Integration:** Interact with the Gemini API following best practices for error handling, rate limiting, and prompt engineering.
*   **Documentation:** Document your code clearly, especially complex logic or public APIs.

## 5. Issue Reporting

When reporting a bug, please provide as much detail as possible:

*   **Clear Title:** Summarize the issue concisely.
*   **Steps to Reproduce:** Detailed, step-by-step instructions.
*   **Observed Behavior:** What happened.
*   **Expected Behavior:** What should have happened.
*   **Environment:** Browser version, OS, extension version.
*   **Screenshots/Logs:** Attach any relevant visuals or console logs.

Use the provided issue templates (`.github/ISSUE_TEMPLATE/bug_report.md`).

## 6. Code of Conduct

This project adheres to a Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to the maintainers.

## 7. Licensing

All contributions will be licensed under the `CC BY-NC 4.0` license. By submitting a pull request, you agree that your contributions will be licensed under this license.

---