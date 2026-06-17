# Security Policy

## Our Approach

TapLaunch is designed as a local macOS utility with a narrow scope. It is built to avoid microphone access, camera access, keyboard input tracking, trackpad click tracking, and cloud connectivity for core functionality.

The local sensor helper only reads on-device motion sensor reports and sends tap event signals back to the TapLaunch app. It does not open apps, run scripts, or connect to the internet.

## Reporting a Security Issue

If you believe you have found a security vulnerability in TapLaunch, please report it privately.

**Email:** [info@asmlab.agency](mailto:info@asmlab.agency)

Please do **not** open a public GitHub issue for security vulnerabilities. Public disclosure before we have had a chance to investigate may put users at risk.

## What to Include

To help us investigate quickly, include as much of the following as possible:

- TapLaunch version (for example, `v1.0.0`)
- macOS version
- MacBook model
- A clear description of the issue
- Steps to reproduce the problem
- Impact assessment, if known
- Any proof-of-concept details or logs that are safe to share

## What to Expect

- We aim to acknowledge receipt of your report within **5 business days**.
- We will investigate valid reports and work on a fix or mitigation as appropriate.
- We may follow up for additional information.
- We will coordinate disclosure timing with you when possible.

## Safe Harbor

We appreciate responsible disclosure. If you act in good faith, follow this policy, and avoid privacy violations, destruction of data, or service disruption, we will not pursue legal action related to your research.

## Supported Versions

Security fixes are provided for the latest public release available on [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases). We recommend always using the latest version.

## General Security Reminders

- Download TapLaunch only from the official [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases) page.
- Verify you are installing `TapLaunch.dmg` from `https://github.com/asmrayat/TapLaunch/`.
- Do not share your administrator password with third parties when installing the local sensor helper.

## Contact

Security reports: [info@asmlab.agency](mailto:info@asmlab.agency)

General support: [info@asmlab.agency](mailto:info@asmlab.agency)
