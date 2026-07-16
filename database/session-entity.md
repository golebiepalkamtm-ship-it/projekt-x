# Entity: Session

**Owner:** Identity. A session represents a revocable authenticated access grant. It contains account reference, issued/expiry/revoked timestamps, authentication assurance, client fingerprint summary, token-family reference, and risk flags.

Only hashed refresh-token material is stored. Sessions are indexed by account and active expiry for revocation. Security events invalidate related sessions without exposing session data to ordinary support staff.
