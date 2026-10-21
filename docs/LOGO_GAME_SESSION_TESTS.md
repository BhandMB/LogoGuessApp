# LogoGuessApp Session Test Plan

Use this plan to verify a complete game session after changes to questions, scoring, or navigation.

- [ ] A new session starts with the expected score and progress.
- [ ] Correct answers update score and progress according to the rules.
- [ ] Incorrect answers do not award unintended points.
- [ ] Repeated clicks or submissions do not score the same question twice.
- [ ] Advancing the question updates the displayed prompt and answer state.
- [ ] Restart behavior resets the intended session data.
- [ ] End-of-game summary matches the answers given.
- [ ] Missing question content is handled without crashing the session.
- [ ] Keyboard and narrow-screen interactions remain usable.
- [ ] A mixed-answer session is tested from start to finish.