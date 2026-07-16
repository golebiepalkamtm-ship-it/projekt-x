# Data Access Matrix

| Data class | Participant | Support | Safety reviewer | Administrator | Service |
|---|---|---|---|---|---|
| Own profile private fields | scoped read/write | limited purpose read | only case-relevant | exceptional only | owning domain |
| Public profile projection | permitted read | permitted read | permitted read | permitted read | discovery projection |
| Verification evidence | no raw access | no | approved review only | break-glass | identity only |
| Safety case evidence | own submitted context only | limited | assigned case | exceptional only | safety only |
| Ledger postings | own scoped view | support view by purpose | no default | controlled | commerce only |
| Audit events | no | no default | case-scoped | incident-scoped | operations only |
