# Eventing Contract

Events report facts in past tense. They contain a stable event name, opaque event ID, schema version, occurred-at timestamp, producer, correlation ID, subject reference, and minimal payload.

Consumers are idempotent and tolerate duplicate, delayed, missing, and out-of-order delivery. Producers use an outbox pattern so a committed state change and its event cannot diverge. Event payloads must not carry Restricted data unless a documented consumer purpose and encryption boundary exist.

Events are additive by default. Breaking schema changes require a new version and a migration period.
