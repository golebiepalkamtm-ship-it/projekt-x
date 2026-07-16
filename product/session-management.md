# Session Management

Sessions are bound to an account, authentication strength, issued time, expiry, and revocation state. Risk-sensitive actions require appropriate authentication freshness. Tokens are short-lived, scoped, rotated, and invalidated server-side after account recovery, credential changes, or security enforcement.

Users can inspect and revoke sessions. Operators cannot impersonate users through ordinary tools; approved break-glass access is separately controlled and audited.
