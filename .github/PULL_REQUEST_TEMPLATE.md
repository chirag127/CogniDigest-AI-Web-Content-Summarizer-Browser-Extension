# 🚀 Pull Request: ContextLens Feature/Fix Submission

**Reviewer Focus:** Please prioritize verification against the architectural standards defined in the repository's `AGENTS.md`.

---

## 1. Description of Change

<!-- Briefly explain the core purpose of this PR. What problem does it solve, or what feature does it introduce? -->

## 2. Motivation and Context

<!-- Why is this change necessary? Link to any relevant issues (e.g., `Closes #123`). -->

## 3. Architectural Alignment (Mandatory Check)

*This section ensures adherence to the Apex Authority Standards.*

- [ ] **SOLID Adherence:** Does this change violate or adhere to SOLID principles? (If a violation was necessary, document why in the comments below).
- [ ] **DRY Enforcement:** Have duplicate logic blocks been consolidated?
- [ ] **Future-Proofing:** Does this utilize current (2025/2026) best practices for browser extensions (e.g., Manifest V3 security, performance optimization)?
- [ ] **Error Handling:** Are all new asynchronous operations and API calls wrapped in robust try/catch or equivalent promise chains?

## 4. Technical Details

<!-- Provide specific technical information necessary for the reviewer. -->

### Technology Stack Specifics (JavaScript/Browser Extension)

*   **Core Logic:** (e.g., New Gemini API call parameters, state management updates, service worker modifications)
*   **UI/UX Impact:** (e.g., Changes to content script injection, resulting DOM manipulation)

## 5. Verification Plan

**How should this PR be tested?**

1.  **Local Build:** `npm run build:prod`
2.  **Local Load:** Load the build artifact into Chrome/Firefox.
3.  **Test Scenario 1:** Navigate to a long-form news article. Verify summary generation speed and accuracy against the prompt configuration.
4.  **Test Scenario 2:** Navigate to a complex Reddit thread (e.g., AskScience or TIFU). Verify thread parsing and summary depth.
5.  **Test Scenario 3 (Negative Test):** Test on a page known to be dynamic or SPA-heavy. Verify graceful degradation or correct content capture.

## 6. Self-Review Checklist

<!-- Ensure all mandatory repository files have been addressed if they were impacted by this change. -->

- [ ] README.md updated (if feature requires new documentation or setup changes).
- [ ] Dependencies updated/locked in `package.json` and verified with `uv` standards (if applicable).
- [ ] CI workflow (`.github/workflows/ci.yml`) integrity maintained.
- [ ] New tests added to cover the modified logic (Vitest/Playwright).

---

**Contributor:** @{{user}}

**Reviewer Guidance:** Please ensure this PR aligns with the high-velocity, zero-defect mandate outlined in the repository's core documentation.