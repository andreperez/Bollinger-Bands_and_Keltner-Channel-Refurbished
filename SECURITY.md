# Security Policy

This repository contains a **TradingView Pine Script® v6 indicator**.

Pine Script runs inside TradingView’s sandboxed environment. This means many “traditional” application security risks (servers, databases, remote code execution, etc.) do not apply here. However, we still treat certain issues seriously—especially anything that could mislead users, violate TradingView rules, or introduce unexpected/malicious behavior.

## Supported Versions

| Version | Supported |
| --- | --- |
| `//@version=6` | ✅ |
| `< v6` | ❌ |

Only Pine Script v6 is supported for contributions and security fixes.

## Reporting a Vulnerability

Please **do not** open a public GitHub issue for security-sensitive reports.

Preferred reporting method:

1. Go to the repository on GitHub
2. Open the **Security** tab
3. Click **Report a vulnerability** (Private Vulnerability Reporting)

If “Report a vulnerability” is not available, open a new issue **without sensitive details** and ask maintainers for a private reporting channel.

### What to include

- A clear description of the issue and why you consider it security-relevant
- Steps to reproduce (minimal example)
- Screenshots or short recordings if it’s visual/UI-related
- The TradingView environment where it occurs (symbol, timeframe, replay/realtime)
- Any proposed fix (optional)

## What We Consider a Security Issue (for Pine Script)

Even though this is “just a script”, the following can be security-relevant in practice:

- **Hidden or deceptive behavior** (e.g., logic that behaves differently than described, intentionally misleading signals, obfuscated code meant to conceal intent)
- **Phishing/social engineering content** embedded in code/comments/docs (links asking for credentials, API keys, exchange logins, etc.)
- **Sensitive data exposure** (users pasting secrets into issues, PRs, screenshots, or sample configs)
- **Supply chain risks** (changes that introduce/alter external dependencies such as imported libraries in a suspicious way)
- **Policy violations** that could put users or the project at risk (e.g., attempts to bypass TradingView limitations or house rules)

## Non-Security Issues

Please use regular GitHub issues for:

- Feature requests
- Visual/style suggestions
- Minor calculation differences that are expected by design
- Performance tuning ideas (unless there’s an exploitation angle or clearly malicious intent)

## TradingView Platform Rules

TradingView publishes platform rules and moderation policies (“house rules”) and has its own terms for scripts and content.

- If the concern is primarily about **TradingView platform security**, accounts, billing, or platform abuse, please report it directly to TradingView via their official support channels.
- If the concern is about **this repository’s code or documentation**, use the vulnerability reporting process above.

## Coordinated Disclosure

We aim to respond as soon as practical.

- We may request clarifications or a minimal reproduction.
- If a fix is needed, we prefer coordinated disclosure (private discussion first, public details after a patch is available).

## Safe Contribution Guidelines

- Never add API keys, passwords, exchange credentials, or personal data to the repository.
- Avoid obfuscation. If a fix is complex, prefer clarity over cleverness.
- Keep changes small and reviewable.

Thanks for helping keep this project safe and trustworthy.
