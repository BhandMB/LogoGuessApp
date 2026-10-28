# Logo Guessing Game Mobile Layout QA

**Date:** 2026-10-28  
**Purpose:** Check that the game remains usable on narrow screens and at increased zoom.

## Viewport checks

Review at a narrow mobile width, a typical phone width, tablet width, and desktop width. Use browser zoom and text scaling where available.

## Checklist

- [ ] Logo/image maintains aspect ratio and is not unintentionally cropped.
- [ ] Answer options fit without horizontal scrolling.
- [ ] Touch targets are comfortably spaced and do not overlap.
- [ ] Score and progress indicators remain readable.
- [ ] Feedback does not cover answer controls.
- [ ] Long names wrap without breaking layout.
- [ ] Keyboard focus remains visible when using an external keyboard.
- [ ] Loading and missing-asset states preserve the layout.

## Evidence

Capture viewport size, browser/device, screenshots when useful, and a short description of each issue. Mark each check complete only after testing the actual UI.