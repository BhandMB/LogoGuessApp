# Accessibility Test Guide

Use this checklist when reviewing a new game screen or question flow.

## Interaction
- Every actionable control can be reached and activated without relying only on color.
- Interactive elements have clear labels and distinguishable states.
- Touch targets remain usable on smaller screens.

## Visual feedback
- Correct, incorrect, selected, disabled, and loading states are distinguishable.
- Text remains readable when system font sizing is increased.
- Important feedback is not communicated by color alone.

## Game flow
- A player can identify the current question and available actions.
- Incorrect answers provide understandable feedback.
- Moving to the next round does not leave stale selection state behind.

## Regression pass
Run the checklist on a fresh launch, after rotation/configuration changes where supported, and through at least one complete round sequence.
