# Logo Guess Scoring Rules QA

Date: 2026-11-03

## Rules to verify
- A correct answer awards the documented points exactly once.
- An incorrect answer follows the configured retry or penalty rule.
- Skipping a question applies the documented score behavior.
- A question cannot be scored repeatedly by rapid taps.
- Score never falls below the permitted minimum.
- Restarting a round resets only the state intended by the game rules.

## Test matrix
Test correct, incorrect, blank, case-variant, whitespace-padded, repeated-submit, timeout, and skipped answers. Include boundary questions and a full-round score reconciliation.

## QA record
For each test, capture starting score, action, expected score, actual score, and pass/fail. Align normalization rules with the accepted-answer data rather than silently accepting ambiguous answers.