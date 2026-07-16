---
status: active
owner: product-and-architecture
last_reviewed: 2026-07-16
---

# Project Memory

Project Memory records decisions that change how ESEP is built or operated. It is a compact, chronological companion to ADRs: an ADR explains the choice; this log makes its downstream impact searchable.

| Date | Decision | Why | Affected areas | Source |
|---|---|---|---|---|
| 2026-07-16 | Documentation-first Project OS | A large platform needs durable context before implementation scales. | All domains | ADR-0001 |
| 2026-07-16 | Trust-sensitive features require human override | Automated ranking or enforcement must not become unreviewable authority. | AI, moderation, support, security | ADR-0002 |
| 2026-07-16 | Market-sensitive requirements stay explicit and open | The project must not invent legality, eligibility, or payment rules before accountable approval. | Product, safety, commerce, data | RFC-0001 |
| 2026-07-16 | Product flows are stateful and policy-bound | Journeys must define permissions, edge states, privacy, safety and operational behavior before UI or APIs. | Product, API, testing, data | Product Bible |
| 2026-07-16 | Logical data design precedes ORM schema | Invariants, ownership, access, lifecycle, events and retention must be settled before physical schema work. | Database, API, security, operations | Database Bible |

### Entry format

`date — decision — reason — impact — links — owner — reversal plan`

Entries are never deleted. Superseding decisions link to the previous entry and state the migration consequence.
