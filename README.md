# MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App/ci.yml?style=flat-square)](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App?style=flat-square)](https://codecov.io/gh/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App)
[![License](https://img.shields.io/github/license/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App?style=flat-square)](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App)
[![Language](https://img.shields.io/github/languages/top/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App?style=flat-square)](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App)
[![Tech Stack (TS)](https://img.shields.io/badge/Stack-TypeScript%20%7C%20React%20Native-blue?style=flat-square)]()

<p align="center">
  <a href="https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/⭐-Star%20this%20Repo-FF69B4?style=social&logo=github" alt="Star this Repo"/>
  </a>
</p>

---

**MoodBite** is an advanced cross-platform mobile application engineered to rigorously track daily food consumption and correlate intake patterns with fluctuating emotional states. This project provides deep insights into nutritional psychiatry, enabling users to proactively manage mental well-being through informed dietary choices. The architecture strictly enforces Feature-Sliced Design (FSD) utilizing the modern Expo ecosystem.

## 🗺️ Architecture Overview

This application is structured using Feature-Sliced Design (FSD) for superior scalability, maintainability, and team velocity, ensuring low coupling between domain layers.

mermaid
flowchart TD
    subgraph Mobile App (React Native / Expo)
        A[App Entry Point / Bootstrap] --> B(Shared / Core)
        B --> C{Features / Slices}
        C --> D[Pages / Screens]
        D --> E[Components / UI]
    end

    subgraph FSD Layers
        style C fill:#f9f,stroke:#333,stroke-width:2px
        C -- Connects To --> C1(App / Entry)
        C -- Connects To --> C2(Pages / Screens)
        C -- Connects To --> C3(Features / Domain Logic)
        C -- Connects To --> C4(Entities / Models)
        C -- Connects To --> C5(Shared / Infra & UI Primitives)
    end

    A -. Uses .- C
    C1 -. Renders .- C2
    C2 -. Uses .- C3
    C3 -. Uses .- C4
    C4 -. Uses .- C5


## 📚 Table of Contents

1. [MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App](#moodbite-mood-and-diet-tracker-react-native-mobile-app)
2. [Architecture Overview](#-architecture-overview)
3. [Table of Contents](#-table-of-contents)
4. [Technology Stack](#-technology-stack)
5. [🤖 AI Agent Directives](#-ai-agent-directives) (Critical Alignment)
6. [Development & Setup](#-development--setup)
7. [Contributing Guidelines](#-contributing-guidelines)
8. [License](#-license)

## ⚙️ Technology Stack

| Category | Technology | Version Standard (2025) |
| :--- | :--- | :--- |
| Core Framework | React Native (Expo Managed) | Latest Stable |
| Language | TypeScript | Strict Mode (TS 6.x Equivalent) |
| State Management | Zustand / Context API | Minimal Boilerplate |
| Styling | Styled Components / Theme System | Component-scoped styling |
| Architecture | Feature-Sliced Design (FSD) | Enforced |
| Linting/Formatting | ESLint + Prettier | Standardized |
| Testing | Vitest / React Native Testing Library | Unit & Component Focus |

## 🤖 AI Agent Directives

<details><summary><strong>Apex Agent Protocol & Architecture Alignment (READ FIRST)</strong></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

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
    *   **No Guessing:** Do not hallucinate APIs. Use secure, established health/nutrition databases only.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Mobile Security Practices** (iOS/Android) and **React Native Performance Bottlenecks**.
    *   **Validation:** Use `docfork` to verify *every* React Native/Expo API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex state synchronization flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / MOBILE (TypeScript / React Native)**
    *   **Stack:** This project uses **TypeScript 6.x+** with **React Native (Expo)**. Key tools include **Biome** (Linter/Formatter, replacing ESLint/Prettier where possible for speed) and **Vitest** (for unit/component testing). **Playwright** is reserved for high-level integration testing against simulators if necessary.
    *   **Architecture:** Strictly adheres to **Feature-Sliced Design (FSD)**. Layers must be explicitly separated: `shared`, `entities`, `features`, `pages`. Imports **MUST NOT** violate FSD boundaries (e.g., `features` cannot import from another unrelated `feature` directly; use `entities` or `shared`).
    *   **Mobile Security:** Prioritize secure storage (e.g., `expo-secure-store`) for any user session tokens or sensitive health metrics. Input validation must be performed on both the client and (hypothetical) backend layer.

## 4. VERIFICATION & EXECUTION
*   **Verification Command (Local Build Check):** `npm run build:check` (Assumes CI script includes type-checking and linting).
*   **Verification Command (Testing):** `npm run test`
*   **Architectural Enforcement:** When modifying code, ensure modifications adhere to the SOLID principles, specifically favoring Dependency Inversion (DIP) by abstracting data sources (e.g., using interfaces/types for Mock vs. Production Data Services).

</details>

## 🚀 Development & Setup

This repository adheres to the highest standards of dependency management and tooling.

### Prerequisites
1.  Node.js (LTS - Current)
2.  npm or Yarn/pnpm (Recommended: **pnpm** for workspace optimization)
3.  Expo CLI installed globally.

### Installation Steps

bash
# 1. Clone Repository
git clone https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App.git
cd MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App

# 2. Install Dependencies (Using pnpm for optimal performance)
pnpm install

# 3. Type Check & Lint Verification (Pre-flight check)
pnpm run lint


### Development Scripts

| Script | Command | Purpose |
| :--- | :--- | :--- |
| `start` | `pnpm run start` | Launches the Expo development server. |
| `android` | `pnpm run android` | Builds and runs on an Android emulator/device. |
| `ios` | `pnpm run ios` | Builds and runs on an iOS simulator/device. |
| `test` | `pnpm run test` | Executes Vitest unit and component tests. |
| `typecheck` | `pnpm run typecheck` | Runs the TypeScript compiler for strict type validation. |

## 🤝 Contributing Guidelines

Contributions are welcome under the **CC BY-NC 4.0** license. Please follow the Apex Authority standards:

1.  **Feature Isolation:** All new logic must be introduced within an FSD layer boundary.
2.  **Testing:** All new features require corresponding unit/component tests achieving 100% coverage for that specific unit.
3.  **Code Review:** Adhere strictly to the Pull Request Template.

Refer to the detailed guidelines in `.github/CONTRIBUTING.md`.

## 🛡️ License

This project is open-sourced under the **Creative Commons Attribution-NonCommercial 4.0 International License**.

See the [LICENSE](LICENSE) file for full details.
