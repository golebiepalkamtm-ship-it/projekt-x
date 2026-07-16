# Domain Map

| Domain | Owns | Emits |
|---|---|---|
| Identity | accounts, sessions, verification state | `identity.verified`, `identity.revoked` |
| Profile | public and private profile projections | `profile.published`, `profile.changed` |
| Discovery | indexes, query intent, ranking inputs | `discovery.indexed` |
| Trust & safety | reports, cases, decisions, appeals | `case.opened`, `case.decided` |
| Commerce | orders, refunds, ledger postings | `payment.authorized`, `ledger.posted` |
| Notification | preferences and delivery attempts | `notification.delivered`, `notification.failed` |
