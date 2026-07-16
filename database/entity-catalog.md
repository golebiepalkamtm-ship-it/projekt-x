---
status: draft
owner: data-architecture
last_reviewed: 2026-07-16
---

# Entity Catalog: Foundation

| Entity | Owning domain | Purpose | Sensitive data |
|---|---|---|---|
| Account | Identity | authenticated actor lifecycle | confidential |
| Credential | Identity | authentication factor metadata | restricted |
| VerificationAssertion | Identity | provider or reviewer attestation | restricted |
| Profile | Profile | owned representation and lifecycle | confidential |
| ProfileProjection | Profile | visibility-scoped presentation | depends on fields |
| Report | Trust & Safety | submitted concern | confidential |
| Case | Trust & Safety | governed investigation lifecycle | confidential |
| EnforcementAction | Trust & Safety | policy outcome | confidential |
| Appeal | Trust & Safety | challenge to an action | confidential |
| AuditEvent | Operations | attributable sensitive action | confidential |

Attributes, relations, lifecycle events, retention, and indexes are specified per entity before schema creation.
