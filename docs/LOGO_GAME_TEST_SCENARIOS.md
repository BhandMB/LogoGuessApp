# Logo Guessing Game Test Scenarios

Use these scenarios to review the main gameplay loop and scoring behavior.

## Gameplay
- [ ] A correct answer is accepted and advances the game as designed.
- [ ] An incorrect answer gives clear feedback without corrupting progress.
- [ ] Empty input is handled gracefully.
- [ ] Repeated submissions cannot award points multiple times for one question.
- [ ] Restarting the game resets the intended state.
- [ ] The final score matches the answers accepted during the session.

## Content and interface
- [ ] Every question has a valid logo asset and answer configuration.
- [ ] Missing assets do not break the whole game screen.
- [ ] Input controls and feedback remain usable on narrow screens.
- [ ] Feedback is not communicated by color alone.

## Regression
- [ ] Test a session with all correct answers.
- [ ] Test a session with all incorrect answers.
- [ ] Test mixed answers and repeated clicks.
- [ ] Verify score and progress after restart.