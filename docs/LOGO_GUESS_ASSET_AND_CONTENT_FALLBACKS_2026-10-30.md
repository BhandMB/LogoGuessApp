# Logo Guess Asset and Content Fallbacks
Date: 2026-10-30

Provide meaningful alternative text for informative images, preserve layout on load failure, use a neutral fallback, and never rely on color alone to communicate correctness. Confirm assets have appropriate usage rights and stable paths.

Each question should have a prompt, valid answer, non-empty choices, and exactly one correct choice unless another format is explicitly supported. Reject duplicate option identifiers.

Test missing files, invalid paths, malformed question entries, and slow asset loading. A failed asset should not block answering.

Review guide only; it does not claim the current assets or data have been audited.