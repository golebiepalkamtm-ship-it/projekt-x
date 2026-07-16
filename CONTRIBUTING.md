# Contributing

## Documentation is a product artifact

Write for a future engineer, operator, designer, and auditor who did not attend the discussion. Prefer precise language, examples, and explicit ownership over aspirational prose.

## Required front matter

Every substantive document starts with: status (`draft`, `proposed`, `accepted`, `deprecated`), owner, last reviewed date, and related ADR/RFC identifiers where relevant.

## Change flow

1. Propose material behavior in an RFC or ADR.
2. Review affected domains and add a Project Memory entry.
3. Update contracts, diagrams, test strategy, and runbooks together.
4. Link the implementation change back to its specification.

## Naming

Use lowercase kebab-case filenames. Prefix numbered ADRs and RFCs with four digits. Keep one canonical source for a rule; link rather than duplicate it.
