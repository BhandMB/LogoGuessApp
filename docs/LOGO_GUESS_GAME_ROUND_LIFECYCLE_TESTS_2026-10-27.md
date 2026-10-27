# Logo Guess Game Round Lifecycle Test Plan

**Date:** 2026-10-27  
**Purpose:** Verify predictable behavior from a new round through completion.

## Lifecycle checks

| Event | Expected behavior |
|---|---|
| Start a new round | One valid question is selected and round state is reset |
| Submit a correct answer | Score changes once according to the scoring rule |
| Submit an incorrect answer | Feedback is shown and score follows the documented penalty policy |
| Submit the same answer repeatedly | One attempt is recorded per accepted interaction |
| Reveal or skip a question | Round advances once and does not reuse stale answer state |
| Reach the final question | Game enters a clear completion state |
| Restart | Score, progress, answer selection, and feedback reset consistently |

## Test design

- Use deterministic question fixtures for unit tests rather than depending on random ordering.
- Test empty and malformed question data without crashing the game.
- Assert score, question index, and completion state together after each transition.
- Verify that rapid repeated clicks cannot score the same answer multiple times.
- Keep the UI feedback separate from the underlying scoring rule where practical.

**Status:** Proposed test plan; execution results should be recorded separately.