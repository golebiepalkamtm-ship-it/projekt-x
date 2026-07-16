# Lifecycle State Machines

State machines are owned by their domains and reject invalid transitions at the command boundary.

| Aggregate | States | Key invariant |
|---|---|---|
| Account | pending, active, restricted, closed | closed accounts cannot create sessions |
| Profile | draft, review, published, restricted, archived | only eligible profile versions may publish |
| Case | intake, triage, investigating, decided, appeal, closed | decision requires policy version and reason |
| PaymentIntent | created, pending, authorised, failed, cancelled | terminal state cannot be overwritten |
| LedgerEntry | posted, reversed | posting is immutable; correction compensates |
