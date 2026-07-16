# Environment Strategy

Local, test, staging, and production environments are isolated with separate credentials and controlled data. Production data does not flow into development environments. Staging represents production architecture sufficiently to validate deployment, migration, provider sandbox, observability, and rollback behaviour.

Configuration is versioned by schema, not committed secrets. Feature flags have owners, expiry dates, targeting rules, metrics, and a removal plan.
