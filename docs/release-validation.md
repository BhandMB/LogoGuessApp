# LogoGuessApp Release Validation

Use this checklist before tagging a release or sharing a demo build.

## Build and install

- Build the `app` module with the Gradle wrapper.
- Install on one emulator and one physical device when available.
- Confirm the app launches without a first-run crash.

## Gameplay

- Start a quiz in Easy, Medium, and Hard modes.
- Verify correct answers increment the score exactly once.
- Verify incorrect answers advance the question without changing the score unexpectedly.
- Confirm the result screen shows the final score and supports returning to the home screen.

## Persistence and lifecycle

- Save a score, close the app, reopen it, and confirm the saved value remains.
- Rotate the device during a quiz and confirm the current state is not silently reset.
- Background and resume the app once during a quiz to check lifecycle handling.

## UI quality

- Check text clipping at small and large font scales.
- Verify answer controls have readable labels and touch targets.
- Check dark mode or the supported theme configuration if enabled.

Record the Android version, device profile, build variant, and any failed case in the release notes.