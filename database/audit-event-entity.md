# Entity: Audit Event

**Owner:** Operations. An immutable audit record captures sensitive or privileged activity. Required fields: event ID, actor, actor capability, action, target reference, reason/purpose, outcome, time, source, correlation ID, and policy/configuration version.

Audit events are append-only, partitioned by time, and protected against ordinary mutation. Query indexes support incident/case reconstruction while retaining least-privilege access.
