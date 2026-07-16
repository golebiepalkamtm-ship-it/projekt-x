# Indexing Strategy

Indexes exist for a documented query, uniqueness invariant, or operational recovery task. Every index names its owning entity, query, cardinality expectation, write cost, privacy risk, and monitoring plan.

Avoid indexing free-text private content and sensitive attributes by default. Partial indexes target active state where helpful. Index additions are measured against write latency and storage budgets; unused indexes are removed through a reviewed migration.
