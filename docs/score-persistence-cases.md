# Score Persistence Cases

- A correct answer increments the score once.
- An incorrect answer does not increase the score.
- Moving to the next question preserves the current score.
- Restarting a round resets temporary game state.
- Leaving and reopening the screen does not create duplicate score updates.
- The UI remains usable when the local data store is empty or unavailable.
