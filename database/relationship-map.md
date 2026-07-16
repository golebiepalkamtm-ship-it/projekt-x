# Relationship Map

```mermaid
erDiagram
  ACCOUNT ||--o{ SESSION : owns
  ACCOUNT ||--o{ VERIFICATION_ASSERTION : receives
  ACCOUNT ||--o| PROFILE : owns
  PROFILE ||--o{ PROFILE_REVISION : has
  PROFILE ||--o{ PROFILE_PROJECTION : publishes
  ACCOUNT ||--o{ REPORT : submits
  CASE ||--o{ EVIDENCE_REFERENCE : contains
  CASE ||--o{ ENFORCEMENT_ACTION : decides
  CASE ||--o{ APPEAL : may_receive
  PAYMENT_INTENT ||--o{ LEDGER_POSTING : settles
```

Cross-domain references use stable opaque IDs. Foreign-key enforcement is used where it does not violate domain boundaries; otherwise, referential integrity is maintained through validated commands and reconciliation.
