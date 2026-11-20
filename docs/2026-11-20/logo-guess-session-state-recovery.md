# LogoGuess Session State Recovery

Date: 2026-11-20

## Goal

Define how a quiz session behaves if the app closes, reloads, or loses focus unexpectedly.

## State to consider

Persist only the minimum needed to resume: session identifier, question index, score, answered-question references, and a version marker. Avoid persisting unnecessary personal information.

## Recovery rules

- Validate persisted data before restoring it.
- Handle unknown schema versions with a safe reset or migration.
- Prevent an already-scored answer from being counted twice.
- Define whether a timed round resumes, pauses, or restarts.
- Clear completed or expired session state according to product behavior.

## Test checklist

- [ ] App reload restores a valid in-progress session.
- [ ] Corrupted state fails safely.
- [ ] Duplicate answer submission does not duplicate score.
- [ ] Version mismatch follows documented recovery behavior.
- [ ] Completed sessions do not reopen unexpectedly.

## Scope

Behavior specification only; no persistence implementation or tests are claimed.