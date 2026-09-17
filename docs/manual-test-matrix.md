# LogoGuessApp Manual Test Matrix

Use this matrix before releasing a build. Record the Android version, device/emulator, result, and any issue link.

| Area | Scenario | Expected result |
|---|---|---|
| Launch | Start app with no saved score | Main screen loads without crash |
| Navigation | Open game from each difficulty | Correct question set is loaded |
| Answering | Select the correct answer | Score increases and next question is shown |
| Answering | Select an incorrect answer | Score remains consistent and feedback is shown |
| Persistence | Finish a round and restart app | Saved score is still available |
| Rotation | Rotate during a round | Current question/state is preserved or safely restarted |
| Accessibility | Use TalkBack on buttons and answers | Controls have meaningful labels and focus order |
| Small screen | Run on a small emulator | Text and buttons remain usable |
| Large screen | Run on a tablet-sized emulator | Layout remains readable without clipping |

## Exit criteria

- No crash in the core game flow.
- All three difficulty modes are playable.
- Score persistence behaves consistently across a cold restart.
- Any known failure is documented before release.
