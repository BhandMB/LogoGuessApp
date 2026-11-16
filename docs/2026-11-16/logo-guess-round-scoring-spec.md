# Logo Guess Round Scoring Specification

## Rules to define
Document points per correct answer, whether attempts affect score, treatment of skipped questions, and the behavior at round completion.

## Consistency
A question should contribute to the score at most once. Repeated submissions and refreshes must not award duplicate points.

## Test cases
Cover correct and incorrect answers, skipped questions, duplicate submissions, final-question completion, and session restoration. Verify that displayed score matches the stored round result.