# LogoGuess Mobile Layout QA

## Scope
Review the game on narrow mobile viewports, including the question image, answer controls, hints, score display, and navigation.

## Layout checks
- No horizontal page overflow at supported viewport widths.
- Logo images preserve aspect ratio and remain legible.
- Answer controls have comfortable touch targets and clear pressed/disabled states.
- Long brand names wrap without covering adjacent controls.
- Score and progress remain visible without obscuring gameplay.
- Dialogs and result screens fit within the viewport and can be dismissed.

## Interaction checks
Test touch input, device rotation, keyboard appearance, slow image loading, and returning from a backgrounded tab.

## Evidence
Capture viewport dimensions, device/browser, screenshots, defects, and retest results. Mark untested device combinations as unknown rather than passed.