---
status: draft
owner: product
last_reviewed: 2026-07-16
---

# Profile Specification

A profile has a public projection, private owner controls, and verification assertions. Fields are classified by visibility: public, audience-limited, private-to-owner, or operator-restricted. Publication is a state transition, not a boolean update.

## Minimum states

`draft` → `ready_for_review` → `published` → `restricted` → `archived`. A participant can return a draft to editing. A restriction requires a reason, expiry or review date, notification policy, and appeal eligibility.

## Rules

- Owners preview the exact public projection before publishing.
- Visibility changes take effect in search, cache, and share previews within a documented propagation target.
- Verification badges state what was verified and when; they do not imply a broad safety guarantee.
- Private media and contact data are never included in public search indexes.
