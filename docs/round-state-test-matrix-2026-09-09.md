# Round State Test Matrix

Verify the game transitions cleanly through these states:

- New round shows one prompt and accepts one answer.
- Correct answer increments the score once and advances the round.
- Incorrect answer shows feedback and advances or retries according to the documented rule.
- Repeated taps do not submit the same answer twice.
- Rotation or activity recreation preserves the current round state.
- End-of-game displays the final score and offers a predictable restart path.

Use deterministic fixtures for logos and expected answers so failures are reproducible.