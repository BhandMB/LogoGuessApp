# Android Release Checks — 2026-09-07

- Launch the app on a clean install and an upgrade install.
- Verify the main game screen renders without clipped controls.
- Rotate through supported orientations and confirm state is preserved as intended.
- Test a correct guess, an incorrect guess, and a completed round.
- Confirm restart/new-round behavior clears only the expected state.
- Check that offline use does not crash when assets are already bundled.
- Review log output for unexpected exceptions before tagging a release.