# Score Calculation Rules

Score updates should be deterministic and easy to verify.

## Rules
- Award points exactly once for a correct answer.
- Do not change the score for an invalid or unanswered submission unless the product rules explicitly say so.
- Keep score updates tied to the current round identifier to prevent stale callbacks from changing a later round.
- Display the updated score only after the state change succeeds.

## Tests
Cover correct answers, incorrect answers, repeated submissions, round transitions, app recreation where supported, and stale-event protection.