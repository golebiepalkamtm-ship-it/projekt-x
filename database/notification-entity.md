# Entity: Notification

**Owner:** Notification. Notification records purpose, recipient, event reference, template/version, delivery channel, preference decision, idempotency key, state, attempts, and provider reference.

The body is generated at delivery time where possible; stored content follows classification and retention rules. Unique `(recipient, purpose, correlation)` constraints prevent duplicate critical messages.
