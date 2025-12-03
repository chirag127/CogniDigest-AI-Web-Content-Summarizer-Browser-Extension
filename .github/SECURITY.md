# Security Policy

At `CogniDigest-AI-Web-Content-Summarizer-Browser-Extension`, we prioritize the security and privacy of our users. We are committed to maintaining a robust and secure browser extension that leverages AI responsibly. This document outlines our security policy and provides guidance for reporting vulnerabilities.

## 1. Reporting a Vulnerability

We appreciate the efforts of security researchers and the community in helping us maintain a secure product. If you discover a security vulnerability, please report it to us immediately and responsibly.

**Please DO NOT open a public GitHub issue.**

To report a vulnerability, please email us directly at:

✉️ **security@chirag127.dev**

### When reporting, please include the following information:

*   **Clear description:** A detailed explanation of the vulnerability, its impact, and potential exploit scenarios.
*   **Reproduction steps:** Precise steps to reproduce the vulnerability. This is crucial for us to validate and fix the issue.
*   **Affected versions:** Specify which versions or branches of `CogniDigest-AI-Web-Content-Summarizer-Browser-Extension` are affected.
*   **Proof-of-Concept (PoC):** If available, provide any code, scripts, or URLs that demonstrate the vulnerability.
*   **Your contact details:** We may need to reach out for more information.

### Our Commitment:

Upon receiving your report, we will:

1.  Acknowledge receipt of your report within **48 hours**.
2.  Investigate the vulnerability thoroughly.
3.  Provide a preliminary assessment and estimated resolution timeline within **5 business days**.
4.  Keep you informed of our progress throughout the remediation process.
5.  Notify you when the vulnerability has been addressed and a fix has been deployed.

## 2. Responsible Disclosure

We kindly request that you adhere to the following responsible disclosure principles:

*   **Private Disclosure:** Do not disclose the vulnerability publicly (e.g., on social media, blogs, or forums) until we have had a reasonable opportunity to address it.
*   **No Harm:** Do not intentionally exploit the vulnerability beyond what is necessary to demonstrate it. Avoid accessing or modifying user data, disrupting services, or engaging in any destructive activities.
*   **Good Faith:** Act in good faith to protect our users' data and privacy.

## 3. Security Best Practices for Contributors

All contributions to `CogniDigest-AI-Web-Content-Summarizer-Browser-Extension` must adhere to strict security guidelines.

*   **Input Validation:** Always validate and sanitize all user input and external data to prevent common vulnerabilities like XSS, injection attacks, and data corruption.
*   **Least Privilege:** Design and implement features with the principle of least privilege. Only request and utilize the minimum necessary browser permissions in the `manifest.json`.
*   **Content Security Policy (CSP):** Maintain a strict CSP within `manifest.json` to mitigate cross-site scripting (XSS) and data injection attacks. Avoid `unsafe-inline` and `unsafe-eval` as much as possible.
*   **Dependency Management:** Regularly update dependencies to their latest secure versions. Utilize tools for scanning known vulnerabilities in third-party libraries.
*   **API Key Management:** Do not hardcode API keys or sensitive credentials directly into the codebase. Use secure environment variables or other secure configuration methods.
*   **Secure Storage:** Handle sensitive user data (if any) with extreme care, using appropriate browser storage APIs and encryption where necessary.
*   **Code Review:** All pull requests are subject to thorough code review, with a focus on potential security implications.
*   **Data Handling:** Be mindful of privacy. Minimize data collection and ensure all data processing complies with relevant privacy regulations.
*   **LLM Interaction Security:** Implement robust error handling and rate limiting when interacting with Large Language Models (LLMs) to prevent abuse or unexpected behavior. Sanitize inputs and outputs to LLMs to avoid prompt injection or data leakage.

## 4. Maintainer Security Guidelines

Project maintainers are responsible for:

*   Ensuring that all reported vulnerabilities are addressed promptly.
*   Conducting regular security audits and dependency scans.
*   Keeping all development environments secure and up-to-date.
*   Communicating security updates and fixes to the community.
*   Following secure release practices for new versions of the extension.

Thank you for helping us keep `CogniDigest-AI-Web-Content-Summarizer-Browser-Extension` secure for everyone.

---

*Last Updated: December 2025*
