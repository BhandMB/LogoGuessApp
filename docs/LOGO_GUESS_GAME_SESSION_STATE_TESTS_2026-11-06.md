# Logo Guess Game Session State Test Plan

Date: 2026-11-06

## State transitions
Verify transitions between start, active question, answered, next question, completed, and restart states.

## Scenarios
- Refresh during an active round.
- Navigate away and return.
- Submit an answer twice quickly.
- Reach the final question.
- Restart after completion.
- Attempt to advance while an answer is still being evaluated.

## Assertions
Question index stays within bounds, score is not duplicated, completed rounds cannot accept further answers, and restart behavior matches the documented persistence policy.

If progress is stored locally or remotely, test corrupted, missing, and stale saved state. Record actual behavior before making product claims.