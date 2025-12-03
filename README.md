# CogniDigest-AI-Web-Content-Summarizer-Browser-Extension

A high-performance, Manifest V3 browser extension utilizing TypeScript and Vite to provide instant, intelligent summaries of web articles and threads via integrated Large Language Models.

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension)
[![Tech Stack](https://img.shields.io/badge/TypeScript-Vite-TailwindCSS-Biome-Vitest-Playwright-blue.svg?style=flat-square)](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension)
[![Lint/Format](https://img.shields.io/badge/Biome-v1.7.0-informational.svg?style=flat-square)](https://biomejs.dev/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgray.svg?style=flat-square)](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension?style=flat-square&logo=github)](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/stargazers)

--- 

**Star ⭐ this Repo!** 

--- 

## 🚀 Project Overview

**CogniDigest** is a cutting-edge, Manifest V3 browser extension built with TypeScript and Vite, designed to deliver swift, AI-powered summaries of web content. Leveraging advanced Large Language Models (LLMs), it transforms lengthy articles, blog posts, and online discussions into concise, digestible insights, enhancing productivity and information consumption.

## 🌳 Architecture

This project adopts a modern, modular architecture optimized for performance and maintainability within the browser extension environment. 

mermaid
graph TD
    A[Browser Extension Core] --> B{Content Script}
    A --> C{Background Service Worker}
    A --> D{Popup UI}
    A --> E{Options UI}
    B --> F[Web Page Content Analysis]
    C --> G[LLM API Integration]
    F --> G
    G --> C
    C --> B
    C --> D
    C --> E
    D --> C
    E --> C


## 🗺️ Table of Contents

*   [🚀 Project Overview](#-project-overview)
*   [🌳 Architecture](#-architecture)
*   [📦 Key Features](#-key-features)
*   [🛠️ Tech Stack](#-tech-stack)
*   [💡 AI Agent Directives](#-ai-agent-directives)
*   [⚙️ Development Setup](#-development-setup)
*   [📜 Project Principles](#-project-principles)
*   [✅ Verification Commands](#-verification-commands)
*   [📄 License](#-license)
*   [🤝 Contributing](#-contributing)
*   [🐞 Bug Report](#-bug-report)
*   [🔒 Security](#-security)

## 📦 Key Features

*   **AI-Powered Summarization:** Instantly generate concise summaries of web articles, news, and social media threads.
*   **Manifest V3 Compliance:** Built with the latest browser extension standards for enhanced security and performance.
*   **TypeScript & Vite:** Leverages a modern, fast development stack for optimal build times and developer experience.
*   **LLM Integration:** Seamlessly connects with popular Large Language Models for intelligent text processing.
*   **User-Friendly Interface:** Intuitive popup and options pages for easy interaction.

## 🛠️ Tech Stack

*   **Language:** TypeScript 6.x
*   **Build Tool:** Vite 7 (with Rolldown)
*   **Extension Framework:** WXT (Web Extension Tooling)
*   **UI Framework:** TailwindCSS v4
*   **Linting & Formatting:** Biome (v1.7.0)
*   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
*   **Architecture:** Feature-Sliced Design (FSD) adapted for Browser Extensions.

---

<details>
<summary>🤖 AI Agent Directives</summary>

## 🤖 AI AGENT DIRECTIVES: COGNIDIGEST 2025.12

**Version:** December 2025 Edition

### 1. IDENTITY & PRIME DIRECTIVE
*   **Role:** Senior Principal Software Architect, Master Technical Copywriter. **40+ years elite experience.**
*   **Context:** December 2025. Building for 2026 standard.
*   **Output Standard:** **EXECUTION-ONLY**. No plans, only executed code/docs.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **Speech-to-Text Interpretation:** **STRICTLY FORBIDDEN** from executing literal typos. **INFER** technical intent semantically based on project context (SSOT is `README.md`).
*   **Mandatory MCP Instrumentation:**
    *   No Guessing. Use `linkup`/`brave` for **Dec 2025 Industry Standards**, **Security Threats**, **2026 UI Trends**.
    *   Verify *every* external API signature using `docfork`.
    *   Use `clear-thought-two` to architect complex flows *before* code generation.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **THIS REPOSITORY: EXTENSION (TypeScript)**
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), WXT (Web Extension Tooling), TailwindCSS v4.
    *   **State Management:** Signals (Standardized).
    *   **Lint/Test:** Biome (Speed) + Vitest (Unit) + Playwright (E2E).
    *   **Architecture:** Feature-Sliced Design (FSD) adapted for Browser Extensions.

### 4. CODE GENERATION & MODIFICATION PROTOCOLS
*   **Syntactic Correctness:** **MUST** produce valid, executable code in the specified language (TypeScript).
*   **Idiomatic Style:** Adhere to language-specific best practices and the **Biome** formatting standard.
*   **SOLID Principles:** Apply Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles rigorously.
*   **DRY Principle:** **MUST NOT** duplicate code. Leverage abstractions and reusable components.
*   **YAGNI Principle:** **MUST NOT** over-engineer. Implement only what is necessary for current requirements.
*   **Error Handling:** Implement robust error handling for all I/O operations, network requests, and external API calls. Use `try...catch` blocks and provide meaningful error messages.
*   **Security:** Prioritize security. Sanitize all user inputs. Avoid storing sensitive data unencrypted. Be mindful of potential XSS, CSRF, and injection vulnerabilities, especially when interacting with web content or external APIs.

### 5. TESTING & VERIFICATION
*   **Unit Tests:** Write comprehensive unit tests using **Vitest** for core logic, utility functions, and component behavior. Aim for >80% code coverage.
*   **Integration Tests:** Develop integration tests to verify the interaction between different modules and services (e.g., UI interactions with background service workers).
*   **End-to-End (E2E) Tests:** Implement E2E tests using **Playwright** to simulate real user scenarios across different browser environments.
*   **Linting & Formatting:** **MUST** auto-format code using **Biome** before committing. All code submitted **MUST** pass Biome linting checks.
*   **CI/CD:** Ensure all changes pass automated checks in the **GitHub Actions CI pipeline** before merging.

### 6. METADATA & DOCUMENTATION
*   **Naming Convention:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>` (e.g., `CogniDigest-AI-Web-Content-Summarizer-Browser-Extension`).
*   **README:** Maintain an up-to-date, comprehensive `README.md` following the **Apex README Replication Protocol**.
*   **AGENTS.md:** This document serves as the directive for AI agents interacting with this repository.
*   **LICENSE:** Use `CC BY-NC 4.0`.

</details>

## ⚙️ Development Setup

**Prerequisites:**
*   Node.js (v20.x or higher)
*   npm or Yarn (recommended: pnpm)

**Installation:**

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension.git
    cd CogniDigest-AI-Web-Content-Summarizer-Browser-Extension
    

2.  **Install dependencies:**
    bash
    # Using pnpm (recommended)
    pnpm install

    # Or using npm
    # npm install
    

## Scripts

| Script          | Description                                     |
| :-------------- | :---------------------------------------------- |
| `:build`        | Build the extension for production.             |
| `:dev`          | Run the extension in development mode.          |
| `:lint`         | Run Biome linter and formatter.                 |
| `:test`         | Run Vitest unit and integration tests.          |
| `:test:e2e`     | Run Playwright end-to-end tests.                |
| `:preview`      | Locally preview `dist` build (if applicable).   |

**Example Commands:**

*   **Start development server:**
    bash
    pnpm run dev
    

*   **Run linters and formatters:**
    bash
    pnpm run lint
    

*   **Run all tests:**
    bash
    pnpm run test
    

## 📜 Project Principles

*   **SOLID:** Adherence to all five SOLID principles for robust and maintainable code.
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code through abstraction and composition.
*   **YAGNI (You Aren't Gonna Need It):** Implement features only when they are required, avoiding premature complexity.
*   **KISS (Keep It Simple, Stupid):** Prioritize simplicity in design and implementation.
*   **Security First:** Integrate security considerations at every stage of development.

## ✅ Verification Commands

*   **Linting & Formatting:** `pnpm run lint`
*   **Unit & Integration Tests:** `pnpm run test`
*   **End-to-End Tests:** `pnpm run test:e2e`
*   **Build:** `pnpm run build`

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/LICENSE) file for more details.

## 🤝 Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/.github/CONTRIBUTING.md) file for guidelines.

## 🐞 Bug Report

If you encounter any bugs, please file a detailed report using the [Bug Report template](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/issues/new?template=bug_report.md).

## 🔒 Security

For security-related issues, please refer to our [SECURITY.md](https://github.com/chirag127/CogniDigest-AI-Web-Content-Summarizer-Browser-Extension/blob/main/.github/SECURITY.md) guidelines.