# Logo Guess Progress Persistence Specification

## State to define
Document which round data persists: current question, answered questions, score, selected difficulty, and completion status.

## Consistency rules
A submitted answer must be applied at most once. Restoring a session must not duplicate points or skip unanswered questions unexpectedly.

## Failure handling
Define behavior for unavailable storage, corrupted saved state, and version changes to the question bank. Provide a safe way to start a fresh round.

## Tests
Save and restore mid-round, refresh after answer submission, restore completed rounds, and load malformed or older state.