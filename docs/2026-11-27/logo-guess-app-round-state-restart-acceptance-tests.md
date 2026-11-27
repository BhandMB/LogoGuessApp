# Round state and restart acceptance tests

## State model
A round has one authoritative state: ready, active, answered, completed, or abandoned. Define allowed transitions and reject invalid actions.

## Acceptance scenarios
1. Starting a round initializes question, timer, and score exactly once.
2. Correct answer awards configured score once.
3. Wrong answer follows documented retry/advance rule.
4. Timer expiry cannot race with answer submission to award duplicate points.
5. Restart clears round state and stale feedback.
6. Navigation follows documented persistence policy.
7. Repeated taps cannot advance multiple questions unexpectedly.

## Evidence
Use deterministic question fixtures and a controllable clock where possible. Assert visible state and underlying score/question index. Include small-screen interaction checks.
