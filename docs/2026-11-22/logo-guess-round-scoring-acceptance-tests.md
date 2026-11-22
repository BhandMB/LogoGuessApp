# LogoGuess Round Scoring Acceptance Tests

Date: 2026-11-22

## Purpose
Define observable scoring behavior for quiz rounds.

## Scoring rules to document
Specify points for correct answers, hints, skipped questions, and time bonuses. Define whether answer matching is case-insensitive, how whitespace is normalized, and whether alternate accepted spellings are supported.

## Acceptance scenarios
- Correct answer receives the documented score once.
- Incorrect answer does not receive correct-answer points.
- Hint usage applies the documented adjustment.
- A skipped question follows the documented scoring rule.
- Repeated submission cannot score the same question twice.
- Round completion calculates the total from recorded question outcomes.

## Edge cases
Test empty answers, leading/trailing spaces, punctuation, alternate spellings, and score boundaries. Keep scoring logic independent from presentation text where possible.

## Scope
Acceptance-test design only; no scoring implementation or test result is claimed.