# Security Policy

## Supported Versions

We actively support and patch the latest stable version of the MoodBite application. Security vulnerabilities in older, unsupported versions may not be addressed.

| Version | Supported |
|---|---|
| Latest (Current Release) | YES |
| Previous Release | YES |
| Older Releases | NO |

## Reporting a Vulnerability

We take security very seriously. If you find a vulnerability in MoodBite, please report it to us as soon as possible through one of the following channels:

1.  **GitHub Security Advisory:** Submit a vulnerability report via the GitHub Security tab for this repository. This is the preferred method for sensitive disclosures.
    *   [Submit a Security Advisory](https://github.com/chirag127/MoodBite-Mood-And-Diet-Tracker-React-Native-Mobile-App/security/advisories/new)

2.  **Email:** Send a detailed report to `security@example.com`. Please use a descriptive subject line, such as "Security Vulnerability Report - [Brief Description]". We will acknowledge receipt of your report within 48 hours.

**When reporting a vulnerability, please include:**

*   A clear and concise description of the vulnerability.
*   Detailed steps to reproduce the vulnerability.
*   The environment in which you discovered the vulnerability (e.g., device, OS version, app version).
*   Any potential impact of the vulnerability.
*   Screenshots, logs, or proof-of-concept code, if applicable.

## Vulnerability Handling

We follow these steps when a security vulnerability is reported:

1.  **Triage:** We will triage the vulnerability report to assess its severity and impact.
2.  **Fix:** We will work to develop and test a fix for the vulnerability.
3.  **Disclosure:** Once a fix is available and deployed, we will coordinate responsible disclosure of the vulnerability, crediting the reporter where appropriate.

## Security Best Practices

As outlined in our `AGENTS.md` directives, we strive to adhere to the highest standards of software development:

*   **TypeScript Strictness:** Utilizing `strict: true` in `tsconfig.json` to catch common errors.
*   **Dependency Management:** Regularly updating dependencies using `uv` and scanning for known vulnerabilities.
*   **Code Reviews:** All changes undergo rigorous code review, prioritizing security considerations.
*   **Feature-Sliced Design (FSD):** Employing architectural patterns that promote modularity and reduce the attack surface.
*   **Expo Security:** Leveraging Expo's built-in security features and best practices for mobile development.

We appreciate your efforts in helping to keep the MoodBite community safe.
