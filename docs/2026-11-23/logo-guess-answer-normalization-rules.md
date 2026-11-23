# LogoGuess Answer Normalization Rules

Date: 2026-11-23

## Purpose
Make answer matching fair and predictable without accepting unintended answers.

## Normalization policy
Document whether matching ignores letter case, trims outer whitespace, normalizes Unicode, or accepts punctuation variants. Keep normalization conservative; do not remove meaningful words or accept broad substring matches by default.

## Accepted alternatives
Maintain explicit alternate answers for abbreviations, former brand names, and common spelling variants. Review each alternative to ensure it still identifies the intended answer uniquely.

## Feedback
Show a clear result without revealing the answer before the player submits. Keep the canonical answer separate from display formatting.

## Test checklist
- [ ] Case and whitespace behavior is defined.
- [ ] Unicode and punctuation cases are reviewed.
- [ ] Approved aliases match.
- [ ] Ambiguous aliases are rejected.
- [ ] Repeated submission cannot alter an already finalized score.

## Scope
Content and matching specification only; no answer engine was changed.