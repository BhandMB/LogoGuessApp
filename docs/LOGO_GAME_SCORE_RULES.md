# Logo Guessing Game: Score Rules

Document the scoring behavior implemented by the game so it remains understandable and testable.

## Rules to confirm
- Define how many points a correct answer earns.
- Define whether incorrect answers earn zero points or have a penalty.
- Clarify whether unanswered questions affect the score.
- Specify when the score is updated and when the final score is shown.
- Define what restarting a game resets: score, question index, and answer feedback.

## Test scenarios
- [ ] Correct answer updates score exactly once.
- [ ] Incorrect answer follows the documented scoring rule.
- [ ] Repeated clicks cannot award duplicate points for one question.
- [ ] Advancing to the next question preserves accumulated score.
- [ ] Final score matches the sum of question outcomes.
- [ ] Restart resets score and progress.

Keep the documented rules synchronized with the actual implementation; this file is a checklist, not a substitute for code-level verification.