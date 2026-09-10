# Gameplay Regression Cases — 2026-09-10

## Round lifecycle
- A new round presents one valid logo prompt.
- Answer submission is disabled while the round is loading.
- Correct answers advance the score exactly once.
- Incorrect answers show feedback without advancing twice.
- Restarting a game resets score, timer, and current-round state.

## Device checks
- Rotate or recreate the screen without losing the active round unexpectedly.
- Verify text remains readable on small displays.
- Confirm a missing image or slow asset load produces a recoverable state.
