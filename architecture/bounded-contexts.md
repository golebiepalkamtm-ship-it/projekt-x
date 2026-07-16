---
status: draft
owner: architecture
last_reviewed: 2026-07-16
---

# Bounded Contexts

| Context | Responsibility | Does not own |
|---|---|---|
| Identity | authentication, account lifecycle, verification assertions | public profile content |
| Profile | profile data, visibility, publication state | sessions or risk decisions |
| Discovery | query, filtering, index and recommendation serving | source-of-truth profile records |
| Trust & Safety | reports, cases, evidence, enforcement and appeals | identity documents or payment settlement |
| Commerce | payment intents, orders, ledger and refunds | provider identity verification |
| Communication | consented conversations and message delivery | enforcement policy |
| Operations | operator tooling, configuration and audit views | direct mutation of another context’s data |

Contexts expose versioned APIs and events. A context may read another context’s published projection, never its internal tables.
