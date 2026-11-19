# LogoGuess Scoring and Round State Contract

## Purpose
Specify predictable scoring and round transitions for the logo guessing game.

## Round lifecycle
A round moves through READY, ACTIVE, ANSWERED, and COMPLETED states. Invalid transitions should be rejected rather than silently changing score or question state.

## Scoring rules to define
- Base points for a correct answer.
- Whether hints reduce the available score.
- Whether incorrect attempts are limited.
- How skipped questions are scored.
- How time bonuses or penalties are calculated, if present.
- How ties are resolved in a completed session.

## Integrity
Calculate scores in trusted application logic. Do not accept a client-provided final score as authoritative. Ensure a question can be scored only once per round.

## Tests
Cover correct and incorrect answers, duplicate submissions, hint usage, skipped questions, timeout, final question completion, and restarting a session. Keep scoring examples in the README aligned with the implemented rules.