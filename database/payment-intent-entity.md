# Entity: Payment Intent

**Owner:** Commerce. This aggregate is inactive until commercial approval. It represents an idempotent request to authorise a quoted amount. Attributes include intent ID, actor, quote version, amount/currency, status, provider reference, idempotency key, expiry, and order reference.

Unique actor/key constraints make retries safe. Provider callbacks cannot bypass quote validation, state transition checks, or ledger posting requirements.
