# Game Round State Cases

Verify the round state for these transitions:

| Transition | Expected behavior |
|---|---|
| Start round | Question and timer are initialized |
| Correct answer | Score increases once and the next round is prepared |
| Incorrect answer | Feedback is shown without awarding points |
| Timeout | Round ends safely and the player can continue |
| Restart | Score, question, and timer return to a clean initial state |

These cases help prevent duplicate scoring and stale UI state during rapid interaction.
