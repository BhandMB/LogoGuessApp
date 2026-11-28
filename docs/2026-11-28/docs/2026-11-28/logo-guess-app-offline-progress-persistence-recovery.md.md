# Offline progress persistence and recovery

## Scope
Define what progress is retained when the app is closed, restarted, or used without a network connection.

## Data policy
Persist only the minimum needed for resume: question-set version, current index, score, completed question IDs, and timestamp. Do not store credentials or unnecessary personal information in progress data.

## Recovery behavior
- Validate stored data before loading it.
- Handle missing, malformed, and older-version progress safely.
- Define whether a changed question bank resumes, resets, or offers a migration.
- Make save operations atomic where the platform permits.
- Provide an explicit reset action with confirmation.

## Tests
Simulate app termination during save, corrupted storage, version upgrade, duplicate completion, clock changes, and user reset. Confirm recovery never awards duplicate points or skips questions silently.
