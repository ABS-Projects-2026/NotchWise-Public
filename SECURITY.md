# Security Policy

## Data Architecture

NotchWise stores all data locally on your Mac in a SQLite database within your Application Support directory. No data is transmitted to external servers during normal operation.

The only features that make network requests are:

- **AnkiConnect sync** — communicates with a locally running Anki instance over localhost (127.0.0.1). No data leaves your machine.
- **AI card suggestions** — when explicitly enabled by you, card text is sent to the AI provider's API using your own API key. This feature is opt-in and requires your explicit action.

## Reporting a Vulnerability

If you discover a security vulnerability in NotchWise, please report it responsibly:

**Email:** [support@notchwise.app](mailto:support@notchwise.app)

**Subject line:** `[SECURITY] Brief description of the issue`

Please include:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Your macOS version and NotchWise version

**Do not** report security issues via public GitHub Issues.

## Response

We will acknowledge your report within 48 hours and aim to provide a fix or mitigation plan within 7 days for critical issues.

## Scope

The following are in scope:

- The NotchWise macOS application
- Local data storage and access controls
- Network requests made by the application
- System permission usage (Accessibility, Screen Recording)

The following are out of scope:

- Third-party services (AnkiConnect plugin, Anthropic API)
- The notchwise.app website
- Social engineering attacks
