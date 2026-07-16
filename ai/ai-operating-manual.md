---
status: approved
owner: architecture
last_reviewed: 2026-07-16
---

# AI Operating Manual

Read this document before writing code in this repository. Its rules override defaults unless a written ADR explicitly supersedes them.

## Locked stack

- TypeScript in strict mode; no committed `any`.
- Next.js App Router; Server Actions for mutations and Route Handlers for public API edges.
- PostgreSQL through Prisma; `prisma/schema.prisma` is the physical-model source of truth.
- Transactional outbox for v1 events; do not call another bounded context’s write path directly.
- Money uses integer minor units and `Currency`; never floating point arithmetic.

## Non-negotiable rules

1. Specifications precede implementation. If a feature has no product and data contract, write one or stop.
2. Every sensitive transition writes an `AuditEvent` in the same transaction: enforcement, payout, verification, account state, and privileged PII read.
3. Ledger postings are append-only. Corrections are new balanced postings referencing the corrected record.
4. Verification and enforcement records are immutable; corrections supersede them.
5. A public profile requires a passed `AGE_18_PLUS` verification assertion, enforced server-side at the query/command layer.
6. Never send personal data to logs, analytics, search, or notification content without documented purpose and deletion path; prefer references.
7. A Prisma model change and matching `database/*-entity.md` change land together.
8. No automation may release funds, permanently restrict a participant, or decide eligibility without a human decision actor.

## Conventions

Organise modules as `src/<context>/{commands,queries,events,repo}`. Validate all server inputs with Zod. External callbacks are idempotent. Tests cover each acceptance criterion; state-machine and money rules require automated unit tests.

## Done means

The model agrees with its entity document; input and errors respect contracts; sensitive transitions audit; happy path and policy-violation tests exist.

## Stop and ask

Stop for a new money flow, enforcement type, sensitive-data category, client-bypassed transition, or conflicting documents.
