# Consistency Model

Within an aggregate, commands provide transactional consistency for invariants. Across domains, ESEP uses durable events and compensating actions. User-facing flows reveal pending state when an asynchronous outcome is not final.

Strong consistency is reserved for security boundaries, idempotency records, and financial postings where an eventual outcome could cause harm. Reconciliation jobs detect missed events and projection drift.
