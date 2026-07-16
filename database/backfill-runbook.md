# Backfill Runbook

1. Approve scope, data classification, owner, maintenance window, and success metric.
2. Snapshot counts and define stable cursor/key range.
3. Run a dry-run on representative non-production data.
4. Execute idempotent batches with rate limits, checkpoints, metrics, and error quarantine.
5. Reconcile source/target counts and sampled semantic checks.
6. Retain evidence, close the runbook, and schedule cleanup of temporary state.

Backfills never bypass RLS, audit, or privacy controls without an approved service identity and reason.
