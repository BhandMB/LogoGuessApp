# Logo Guess Game Scoring Regression Plan

**Date:** 2026-10-28  
**Purpose:** Keep scoring behavior stable as game interactions evolve.

## Rules to document

Before writing assertions, record the actual intended values for correct answers, incorrect answers, hints, skips, and unanswered rounds. Avoid embedding assumptions from this template if the game uses different rules.

## Regression cases

- Correct answer updates score exactly once.
- Incorrect answer follows the documented penalty policy.
- Repeated clicks on a locked/completed question do not change score again.
- Hint or skip behavior follows the scoring policy.
- Restart resets score and progress.
- Final-round completion shows the final score and does not advance beyond the question list.
- Empty question data produces a clear fallback state.

## Test approach

Use deterministic question fixtures. Assert score and round state after each action. Cover rapid repeated interactions and keyboard activation in addition to pointer clicks. Record the test command and actual outcome after execution.