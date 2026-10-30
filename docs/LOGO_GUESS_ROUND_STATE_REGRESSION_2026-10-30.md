# Logo Guess Round State Regression
Date: 2026-10-30

Verify a new round initializes score, question index, selected answer, timer, and progress consistently.

Scenarios: start a game; award points only once for a correct answer; apply documented incorrect-answer scoring; ignore repeated clicks during feedback; clear prior selection on next question; show final summary once; restart to a deterministic initial state.

Also test missing question data, duplicate choices, and an empty question collection. A round should have one authoritative state transition per answer.

Regression plan only; no runtime tests are claimed.