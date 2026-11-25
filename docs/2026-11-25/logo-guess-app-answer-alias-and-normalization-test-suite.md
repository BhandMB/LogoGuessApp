# Logo Guess App Answer Alias and Normalization Test Suite

## Objective
Accept reasonable answer variations while avoiding accidental acceptance of unrelated brands.

## Normalization rules to define
- Trim leading and trailing whitespace.
- Normalize repeated internal whitespace.
- Compare case-insensitively.
- Define punctuation handling explicitly.
- Support approved aliases and localized spellings where curated.
- Avoid overly broad substring matching.

## Test categories
- Exact canonical answer
- Uppercase and lowercase
- Leading and trailing spaces
- Repeated spaces
- Approved abbreviation
- Approved alternate spelling
- Punctuation variation
- Similar but incorrect brand name
- Empty answer
- Unicode and accented input

## Content model
Keep canonical answer and accepted aliases with the question record or content pack. Review aliases when questions are added or translated. Do not infer aliases from arbitrary user submissions without moderation.

## Acceptance criteria
All approved aliases pass, near-miss answers fail, and normalization behavior is deterministic across supported browsers and locales.
