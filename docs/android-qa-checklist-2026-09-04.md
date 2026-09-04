# Android QA Checklist — 2026-09-04

- Verify the app starts cleanly after a fresh install.
- Confirm each logo question loads the expected image and answer options.
- Reject incomplete answers with a clear user-facing message.
- Confirm score updates exactly once per submitted answer.
- Test rotation or lifecycle recreation without losing the current question state.
- Verify navigation back and restart flows do not duplicate screens.
