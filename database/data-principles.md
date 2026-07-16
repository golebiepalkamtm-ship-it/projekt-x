---
status: draft
owner: data-architecture
last_reviewed: 2026-07-16
---

# Data Principles

Every record has an owning domain, classification, purpose, retention rule, and access policy. Personal data is not copied to analytics, logs, queues, or search indexes unless the destination has a documented lawful purpose and deletion path.

Business events are immutable facts; mutable projections may be rebuilt. Financial balances are derived from a double-entry ledger, never edited as a standalone number. Identifiers are opaque and never encode sensitive attributes.

Row-level security is defense in depth, not the only authorization layer. Services authenticate, authorize, validate tenant/resource scope, and log sensitive reads before database access.
