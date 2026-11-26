# Logo Guess App Round Timer Pause and Resume Specification

## Objective
Define predictable timer behavior across pauses, tab visibility changes, and app interruptions.

## State model
Represent each round with explicit states such as Ready, Running, Paused, Completed, and Expired. Only valid transitions should be accepted. The exact names should align with the implementation.

## Timing rules
- Start the timer once when a round begins.
- Pause should preserve remaining duration.
- Resume should continue from the preserved remaining duration.
- Expiry should complete the round exactly once.
- Repeated pause or resume actions should be harmless.
- Background-tab behavior must be documented and consistent.

## Accuracy
Prefer a monotonic time source for measuring elapsed duration. Avoid decrementing a counter solely on each UI interval tick, because browser throttling can make the displayed count drift.

## Test scenarios
- Pause immediately after start.
- Resume after a long pause.
- Rapid repeated pause/resume.
- Browser tab hidden and restored.
- Timer expires while the tab is inactive.
- Round completion and answer submission occur at nearly the same time.

## Accessibility
Announce meaningful timer state changes without overwhelming screen-reader users with repeated second-by-second announcements.
