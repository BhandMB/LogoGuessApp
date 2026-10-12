# Logo Guessing Game QA Checklist

## Core gameplay
- [ ] A question displays the expected logo image and answer options.
- [ ] Selecting the correct answer awards the expected score.
- [ ] Selecting an incorrect answer follows the intended feedback flow.
- [ ] Advancing to the next question does not repeat or skip items unexpectedly.
- [ ] The final question transitions to a clear completion state.

## Content and assets
- [ ] Every question has a valid image asset.
- [ ] Image paths and filename casing work on case-sensitive systems.
- [ ] Missing assets fail gracefully rather than breaking the game.
- [ ] Brand names and answer labels are spelled consistently.

## Interface and accessibility
- [ ] Buttons provide visible feedback when selected.
- [ ] Text and controls remain usable on smaller screens.
- [ ] Interactive controls can be reached by keyboard where applicable.
- [ ] Status is not communicated by color alone.

## Regression scenarios
- [ ] Start or restart a game.
- [ ] Answer every question type.
- [ ] Verify score updates and final score.
- [ ] Navigate rapidly between questions.
- [ ] Confirm the restart resets score and question progress.