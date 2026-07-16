# Service Boundaries

The initial implementation may deploy a modular monolith, provided module boundaries follow the bounded-context contract. Splitting is justified by independent scaling, security isolation, deployment cadence, or team ownership—not by a desire for distributed complexity.

Each module declares its commands, queries, emitted events, persistence boundary, error taxonomy, and service-level objectives. Cross-module writes use a command or durable event workflow. Synchronous calls must have timeout, retry classification, idempotency, and fallback behavior.
