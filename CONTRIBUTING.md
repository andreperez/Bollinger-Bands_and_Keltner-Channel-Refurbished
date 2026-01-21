# Contributing

Thanks for your interest in contributing to **Bollinger Bands + Keltner Channel Refurbished**.

This project is a TradingView **Pine Script® v6** indicator. Contributions can include bug reports, feature requests, documentation improvements, and code changes.

## Code of Conduct

By participating, you agree to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Ways to Contribute

- **Report bugs** (logic errors, repainting surprises, performance issues, UI/input problems)
- **Request features** (new band styles, new MA types, better defaults, new visual options)
- **Improve docs** (README clarifications, screenshots, explanations)
- **Contribute code** (fixes, refactors, new features)

If you are unsure where to start, open an issue describing what you want to do and we can discuss the best approach.

## Before You Start

### Scope

Please keep changes focused and incremental:

- One bug fix or one feature per pull request, when possible.
- Avoid large rewrites unless discussed first.

### Project Files

- Main indicator: [Bollinger Bands + Keltner Channel Refurbished.pine](Bollinger%20Bands%20%2B%20Keltner%20Channel%20Refurbished.pine)
- Project overview and examples: [README.MD](README.MD)

## Reporting Bugs

When opening a bug report, include:

- **TradingView symbol** (e.g., BTCUSDT)
- **Chart timeframe** (e.g., 15m, 1h, 1D)
- **Expected behavior** vs **actual behavior**
- Screenshots or short screen recording (if visual)
- Whether it happens on:
  - Historical bars
  - Realtime bars
  - Replay mode
- A minimal set of inputs to reproduce the issue

## Requesting Features

When proposing a feature, describe:

- The problem it solves and why it helps
- Suggested UI/inputs (names, defaults, tooltips)
- Any trade-offs (repainting vs confirmation delay, performance cost)

## Development Setup (Pine Script)

Pine Script runs inside TradingView. A typical workflow is:

1. Open TradingView → **Pine Editor**
2. Paste or import the code from the main `.pine` file
3. Save the script
4. Add it to a chart and validate behavior across symbols/timeframes

### Optional Local Tooling

- VS Code for editing
- A Pine Script extension/linter if you use one

## Code Style and Quality Guidelines

Please follow these rules to keep the codebase consistent and publication-ready:

- Target **Pine Script v6** (`//@version=6`).
- Prefer **self-explanatory names** and avoid unclear acronyms.
- Keep logic reusable by extracting helpers into **functions**.
- Use **explicit types** when variables can be `na`.
- Avoid calling plotting functions from local scope (e.g., no `plot()` inside `if` blocks).
- Use input **groups** and tooltips for non-obvious settings.
- Keep changes performant (cache expensive calculations when possible).

### Repainting and Confirmation

If you add signals or multi-timeframe logic:

- Make repainting behavior explicit and documented.
- Prefer giving users toggles (e.g., “confirm on bar close”) when the feature affects timing.

## Submitting a Pull Request

1. Fork the repository and create a branch:
   - `fix/<short-description>`
   - `feature/<short-description>`
2. Make your changes.
3. Validate:
   - Script compiles in TradingView.
   - No new warnings/errors in your editor.
   - Behavior is correct on multiple symbols/timeframes.
4. Update documentation when needed (README and/or images).
5. Open a pull request with:
   - What changed and why
   - How you tested
   - Screenshots for visual changes

### Pull Request Checklist

- [ ] Code compiles in TradingView
- [ ] Inputs have clear names, defaults, and tooltips
- [ ] No plotting functions in local scope
- [ ] No secrets or personal data added
- [ ] Docs updated if behavior or UI changed

## Security Issues

If you believe you found a security or account-related issue, **do not** open a public issue. Prefer a private report to the maintainer.

## Licensing

Unless stated otherwise in the repository, by submitting a pull request you agree that your contribution can be redistributed under this project’s license.
