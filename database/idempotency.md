# Idempotency Standard

Commands with side effects accept an idempotency key scoped to actor, command type, and request fingerprint. The system stores request outcome or in-progress state long enough to safely retry, returning the original result for a matching request.

Key reuse with a different payload is rejected. Webhooks deduplicate on provider event identity and retain processing evidence. Idempotency state has a retention policy and does not contain unnecessary personal payloads.
