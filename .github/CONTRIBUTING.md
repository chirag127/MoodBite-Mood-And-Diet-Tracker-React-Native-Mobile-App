# Contributing to MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App

Welcome to the Apex Initiative. We strive for **Zero-Defect, High-Velocity, Future-Proof** software. Your contributions are vital to maintaining this standard for this health-tech platform.

## 1. Core Principles: The Apex Mandate

All contributions must align with the following architectural and quality philosophies, as defined by the Apex Technical Authority:

1.  **SOLID Compliance:** Ensure all new components or modifications adhere strictly to the SOLID principles.
2.  **DRY (Don't Repeat Yourself):** Abstraction layers must be leveraged aggressively to prevent code duplication.
3.  **YAGNI (You Ain't Gonna Need It):** Avoid speculative programming. Implement only what is required by the current feature specification or documented bug.
4.  **Feature-Sliced Design (FSD):** All React Native code must respect the established FSD layers (`shared`, `entities`, `features`, `pages`). New features must be implemented at the appropriate slice depth.
5.  **Strict TypeScript:** Maintain rigorous type safety throughout the codebase.

## 2. Development Workflow

We operate on a GitFlow-inspired, feature-branch model, optimized for rapid CI/CD pipeline execution.

### A. Prerequisites (Apex Toolchain)

Before committing, ensure your local environment is set up according to the main repository standards. For this **React Native (Expo/TypeScript)** project, this means:

1.  Node.js (LTS/Current) and npm/yarn/pnpm installed.
2.  Expo CLI installed globally or via `npx`.
3.  `biome` and testing utilities are locally available (ensure running linting via pre-commit hooks).

### B. Branching Strategy

1.  **Fork** the repository `chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App`.
2.  **Clone** your fork locally.
3.  Create a descriptive feature branch from `main`:
    bash
    git checkout -b feature/short-descriptive-name
    # OR
    git checkout -b fix/issue-number-description
    

### C. Code Implementation & Verification

*   **Linting & Formatting:** Run the formatter check **before** committing. Any style violations will cause the CI build to fail.
    bash
    npx @biomejs/biome check --apply . 
    # Or, if using pre-commit hooks, ensure they pass.
    
*   **Testing:** All new features **MUST** include corresponding unit tests (Vitest) and, where applicable, integration/e2e tests (Playwright, if configured for mobile integration testing).
    bash
    npm test # Or your chosen test runner command
    
*   **Commit Hygiene:** Write clear, atomic commits. Follow a standard like Conventional Commits.

## 3. Submitting a Pull Request (PR)

1.  Ensure your branch is **up-to-date** with the upstream `main` branch (rebase preferred over merge).
2.  Push your feature branch to your fork.
3.  Open a Pull Request targeting the `main` branch of `chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App`.
4.  **PR Template:** You **MUST** fill out the provided `PULL_REQUEST_TEMPLATE.md` completely. Pay special attention to referencing affected issues and describing architectural changes.

## 4. Reporting Issues

If you discover a bug or want to propose a new feature, please use the provided templates:

*   **Bug Reports:** Use the `bug_report.md` template in `.github/ISSUE_TEMPLATE/`.
*   **Feature Requests:** Create a new issue using the standard GitHub template, ensuring your proposal details the value proposition and potential architectural impact.

--- 

*This repository is governed by the **CC BY-NC 4.0 License**.*