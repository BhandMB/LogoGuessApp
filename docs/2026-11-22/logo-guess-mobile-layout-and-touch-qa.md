# LogoGuess Mobile Layout and Touch QA

Date: 2026-11-22

## Objective
Review quiz usability on small screens and touch-first devices.

## Layout checks
- Content fits common narrow viewport widths without unintended horizontal scrolling.
- Logo imagery preserves aspect ratio and remains legible.
- Answer controls remain visible when the on-screen keyboard opens.
- Text scales without clipping at increased system font sizes.
- Dialogs and menus remain within the viewport.

## Touch checks
Ensure interactive targets have adequate spacing, provide visible pressed and focus states, and do not rely on hover-only feedback. Avoid placing destructive or round-ending actions next to frequent answer controls.

## Test matrix
Record device/browser, viewport, orientation, zoom, and input method. Include portrait and landscape where supported.

## Checklist
- [ ] Main quiz flow works at narrow widths.
- [ ] Keyboard does not obscure essential controls.
- [ ] Touch targets are usable.
- [ ] Images remain clear and proportionate.
- [ ] Focus and feedback are perceivable.

## Scope
QA checklist only; no device testing was performed.