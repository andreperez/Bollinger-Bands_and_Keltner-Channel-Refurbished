# Feature PR

## Problem / Motivation

What user problem does this solve?

## Proposed Solution

What did you implement?

## User-Facing Changes

- New/changed inputs:
  - Name:
  - Default:
  - Tooltip:
- Affected indicator modes (select all that apply):
  - [ ] Bollinger Bands
  - [ ] Keltner Channel
  - [ ] Parallel Channels
  - [ ] VWAP Bands

## Repainting / Confirmation

If this feature affects signal timing or uses multi-timeframe data, clarify it here:

- Does it repaint on realtime bars?
- Is there a user toggle for confirmation (e.g., confirm on bar close)?
- Any expected delay/trade-offs?

## Validation

- [ ] Script compiles in TradingView (Pine Script v6)
- [ ] Tested on at least 2 symbols:
- [ ] Tested on at least 3 timeframes (e.g., 5m / 1h / 1D):
- [ ] Checked historical + realtime behavior
- [ ] Performance check (no unnecessary repeated heavy calls)

## Screenshots / Examples

Attach screenshots or short clips for visual/UI changes.

## Checklist

- [ ] No plotting functions called in local scope (e.g., no `plot()` inside `if` blocks)
- [ ] Explicit typing used where `na` is possible
- [ ] No secrets, personal data, or phishing links added
- [ ] No intentional obfuscation
- [ ] Docs updated if needed (README, screenshots)
