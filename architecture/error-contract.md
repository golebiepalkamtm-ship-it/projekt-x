# Error Contract

Public interfaces return a stable machine code, human-safe message, correlation ID, and field-level detail only when it does not disclose protected information.

| Class | Example | Client behaviour |
|---|---|---|
| `validation_failed` | invalid input | correct and retry |
| `authentication_required` | expired session | sign in again |
| `forbidden` | missing capability | stop; do not infer resource state |
| `conflict` | stale version or duplicate request | refresh or reuse idempotency key |
| `rate_limited` | threshold exceeded | wait for retry hint |
| `temporarily_unavailable` | provider outage | retry safely |

Internal errors are logged with context but never expose stack traces, secrets, or another participant’s data.
