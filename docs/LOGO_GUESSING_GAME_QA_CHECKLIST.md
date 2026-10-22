# Logo Guessing Game QA Checklist

- [ ] Correct answer advances or completes the round as designed.
- [ ] Incorrect answer gives clear feedback and follows the configured retry rules.
- [ ] Score changes only according to documented game rules.
- [ ] Restart behavior resets the expected session state.
- [ ] End-of-game state prevents unintended extra scoring.
- [ ] Missing or unavailable image assets have a graceful fallback.
- [ ] Interactive controls are usable by keyboard where applicable.
- [ ] Text remains readable at common viewport sizes.
- [ ] Repeated play does not retain stale score or answer state.

Confirm expected behavior against the implementation and record actual test results separately.