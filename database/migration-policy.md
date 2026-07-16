# Migration Policy

Migrations are forward-compatible, reversible where feasible, observable, and rehearsed. Use expand–migrate–contract: add compatible structures, backfill with checkpoints, deploy readers/writers, verify, then remove old structures after all consumers migrate.

Every migration declares owner, affected data class, lock/latency risk, batch strategy, resume key, validation query, rollback/repair plan, backup impact, and communication. Destructive migrations require explicit approval and retention review.
