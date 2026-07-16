# Data Quality Controls

Data quality rules are executable where possible: schema validation, referential checks, state-machine transitions, uniqueness constraints, freshness monitoring, reconciliation, and sampled semantic review.

Every critical quality rule names a source, threshold, owner, alert action, and remediation path. Invalid records are quarantined with a safe reason rather than silently coerced into a false state.
