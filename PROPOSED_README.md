# MoodBite: Mood & Diet Tracker

A sophisticated React Native mobile application designed to meticulously track your daily food intake and correlate it with your mood states. By analyzing these correlations, MoodBite empowers you to uncover dietary patterns that foster enhanced mental well-being and overall wellness.

---

## 🚀 Vision

To be the leading mobile platform for individuals seeking to understand and optimize their diet for improved mental health, leveraging data-driven insights and a user-centric experience.

---

## 🤖 AI AGENT DIRECTIVES

<details>
<summary><strong>AI Agent Directives (December 2025 Edition)</strong></summary>

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO A: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x (Strict)** with **Expo** for React Native development. **Vite 7 (Rolldown)** is the build tool. **Tauri v2.x** is not applicable here as it's a native app framework. **WXT (Web Extension Toolkit)** is also not applicable.
    *   **State Management:** Employ standardized **Signals** for predictable and efficient state updates across the application.
    *   **Linting & Formatting:** Utilize **Biome** for ultra-fast code analysis and formatting, ensuring code quality and consistency across the codebase.
    *   **Testing:** Implement **Vitest** for rapid unit testing and **Playwright** for comprehensive end-to-end (E2E) testing, guaranteeing application stability and user experience.
    *   **Architecture:** Strictly adhere to the **Feature-Sliced Design (FSD)** methodology for a scalable, maintainable, and understandable project structure.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable for this project.***
*   **TERTIARY SCENARIO C: DATA / AI / SCRIPTS (Python) - *Not applicable for this project.***

---

## 4. DEVELOPMENT & DEPLOYMENT STANDARDS (LATE 2025)
*   **Configuration:** Utilize **Expo Config Plugins** and **app.json/app.config.js** for native module configuration and app metadata.
*   **CI/CD:** Integrate **GitHub Actions** for automated builds, testing, and deployments. Leverage Expo Application Services (EAS) Build and Submit for streamlined mobile app distribution.
*   **Security:** Follow **OWASP Mobile Security Project** guidelines. Implement secure storage for sensitive data (e.g., using Expo SecureStore). Regularly audit dependencies for vulnerabilities using tools like `npm audit` or `yarn audit`.
*   **Performance:** Optimize React Native performance through memoization, efficient list rendering (e.g., `FlatList` optimizations), and minimizing re-renders. Profile using native performance tools and React DevTools.
*   **Code Quality:** Enforce **SOLID** principles, **DRY** (Don't Repeat Yourself), and **KISS** (Keep It Simple, Stupid). Prioritize readability and maintainability.

---

## 5. DOCUMENTATION MANDATE
*   **README:** Maintain a comprehensive `README.md` as the project's primary interface.
*   **AGENTS.md:** This document serves as the definitive guide for AI agents interacting with the repository.
*   **CONTRIBUTING.md:** Provide clear guidelines for external contributors.
*   **ISSUE_TEMPLATE:** Standardized templates for bug reports and feature requests.
*   **PULL_REQUEST_TEMPLATE:** Ensure pull requests are well-documented and reviewed.

---
</details>

---

## 🌳 Architecture (Feature-Sliced Design)

mermaid
graph TD
    subgraph Features
        A[Mood Tracking]
        B[Diet Logging]
        C[Analysis & Insights]
        D[User Profile]
    end

    subgraph Entities
        E[Food Item]
        F[Mood Entry]
        G[User Data]
    end

    subgraph App Structure
        H[Main App Entry]
        I[Navigation]
        J[UI Components]
        K[API Services]
        L[Configuration]
    end

    A --> E
    B --> E
    A --> F
    C --> F
    C --> E
    D --> G

    H --> I
    I --> A
    I --> B
    I --> C
    I --> D
    J --> I
    J --> A
    J --> B
    J --> C
    J --> D
    K --> J
    K --> L


---

## 📋 Table of Contents

*   [Vision](#-vision)
*   [AI Agent Directives](#-ai-agent-directives)
*   [Architecture](#-architecture-feature-sliced-design)
*   [Table of Contents](#-table-of-contents)
*   [Key Features](#-key-features)
*   [Tech Stack](#-tech-stack)
*   [Getting Started](#-getting-started)
*   [Development Scripts](#-development-scripts)
*   [Testing](#-testing)
*   [Contributing](#-contributing)
*   [License](#-license)

---

## 🌟 Key Features

*   **Intuitive Mood Logging:** Easily record your daily mood with customizable scales and notes.
*   **Detailed Diet Tracking:** Log food items, quantities, and meal times.
*   **Correlation Analysis:** Visualize the relationship between your dietary habits and mood fluctuations.
*   **Personalized Insights:** Receive data-driven recommendations for dietary adjustments.
*   **User Profile Management:** Securely manage your personal data and preferences.
*   **Cross-Platform:** Runs seamlessly on both iOS and Android devices.

---

## 💻 Tech Stack

*   **Core:** React Native (Expo)
*   **Language:** TypeScript (Strict Mode)
*   **Build Tools:** Vite 7 (Rolldown)
*   **State Management:** Signals
*   **UI Components:** NativeBase / React Native Paper (TBD)
*   **Linting & Formatting:** Biome
*   **Testing:** Vitest (Unit), Playwright (E2E)
*   **Architecture:** Feature-Sliced Design (FSD)

---

## 🚀 Getting Started

### Prerequisites

*   Node.js LTS (v20+ recommended)
*   npm or Yarn
*   Expo CLI (`npm install -g expo-cli`)
*   Git

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App.git
    cd MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App
    

2.  **Install dependencies:**
    bash
    npm install
    # or
    yarn install
    

---

## 🛠️ Development Scripts

| Script        | Description                                        |
|---------------|----------------------------------------------------|
| `npm run start` | Starts the Expo development server.                |
| `npm run dev:ios`| Runs the app on an iOS simulator.                  |
| `npm run dev:android`| Runs the app on an Android emulator/device.       |
| `npm run lint`  | Runs Biome for linting and formatting checks.      |
| `npm run format`| Formats code using Biome.                          |
| `npm run test`  | Runs unit tests with Vitest.                       |
| `npm run test:e2e`| Runs end-to-end tests with Playwright.             |

---

## 🧪 Testing

MoodBite employs a robust testing strategy to ensure quality and reliability:

*   **Unit Tests:** Written using **Vitest**, these tests cover individual components, utility functions, and business logic.
*   **End-to-End (E2E) Tests:** Utilizes **Playwright** to simulate real user interactions across the application, validating critical user flows on both iOS and Android platforms.

Run tests via the development scripts:

bash
# Run all unit tests
npm run test

# Run E2E tests
npm run test:e2e


---

## 🤝 Contributing

We welcome contributions to MoodBite! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines on how to submit bug reports, feature requests, and pull requests.

---

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. See the [LICENSE](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App/blob/main/LICENSE) file for more details.
