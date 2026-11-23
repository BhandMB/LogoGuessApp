# LogoGuess Round Timer and Pause Behavior

Date: 2026-11-23

## Objective
Specify consistent timing behavior across app backgrounding, pauses, and round transitions.

## Policy decisions
Define the duration of each round, whether users may pause, what happens when the app is backgrounded, and whether time continues during network or loading delays. Use a monotonic time source for elapsed-duration measurement where available.

## State handling
Persist the round deadline or remaining duration according to the chosen policy. On resume, validate persisted state and prevent the timer from restarting unintentionally.

## Verification
- [ ] Timer does not gain time after a reload unless policy permits it.
- [ ] Background and foreground behavior is deterministic.
- [ ] Pause and resume preserve the correct remaining time.
- [ ] Round completion fires only once.
- [ ] Timer display and scoring use the same time basis.

## Scope
Behavior specification only; no timer implementation or device test is claimed.