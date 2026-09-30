# Project Maintenance Guide

## Before changing gameplay

1. Identify the affected round state or user interaction.
2. Check the existing gameplay regression and state-case documents.
3. Record the expected behavior before implementation.
4. Verify that restart, lifecycle, duplicate-answer, and score behavior remain consistent.

## Before changing UI

- Check touch-target size and readable text.
- Verify labels and feedback are understandable.
- Re-test the affected screen after rotation or recreation where supported.
- Confirm that the change does not silently alter scoring or answer validation.

## Before release

- Verify the documented gameplay flows.
- Run the available Android build/test process from the local project checkout.
- Review release notes for user-visible behavior changes.
- Keep documentation focused on reproducible checks rather than duplicate daily notes.
