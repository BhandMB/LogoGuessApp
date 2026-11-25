# Logo Guess App Progress Migration and Version Compatibility

## Purpose
Protect saved game progress when the question pack or local storage schema changes.

## Versioning
Store a schema version with saved progress. Keep question identifiers stable across content updates. Do not rely on array position as the permanent identity of a question.

## Migration strategy
1. Read and validate the saved payload.
2. Detect its schema version.
3. Apply a deterministic migration for supported older versions.
4. Preserve compatible scores and completed question IDs.
5. Discard or quarantine malformed data safely.
6. Write the migrated payload only after validation succeeds.

## Compatibility cases
- First launch with no saved data
- Current schema
- Each supported prior schema
- Unknown future schema
- Corrupted JSON
- Question removed from the latest pack
- Duplicate or unknown question identifiers
- Storage quota or write failure

## User experience
If progress cannot be recovered, explain the issue plainly and avoid crashing the app. Provide a safe reset path only after user confirmation.

## Verification
Test migration fixtures from real prior schema versions and confirm repeated migration does not change the result.
