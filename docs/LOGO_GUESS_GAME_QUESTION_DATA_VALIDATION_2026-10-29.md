# Logo Guess Game Question Data Validation Checklist

**Date:** 2026-10-29  
**Purpose:** Prevent malformed question data from breaking game flow.

## Data quality checks

- Each question has a stable unique identifier where the model supports IDs.
- Prompt and answer values are present and non-empty.
- Correct answers match the option set when the question uses multiple choice.
- Duplicate options and duplicate question IDs are handled intentionally.
- Asset references resolve or have a defined fallback.
- Unsupported question types are rejected or safely skipped.
- Text length and special characters do not break the layout.
- An empty dataset produces a clear empty state rather than a crash.

## Test strategy

Create valid, empty, and malformed fixtures. Assert validation outcomes and confirm invalid records cannot corrupt score, progress, or round state. Keep validation separate from rendering where practical.

## Acceptance checklist

- [ ] Dataset format is documented.
- [ ] Validation errors identify the problematic record safely.
- [ ] Tests cover both valid and invalid fixtures.
- [ ] Runtime fallback behavior is deliberate and visible.