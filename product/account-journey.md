---
status: draft
owner: identity
last_reviewed: 2026-07-16
---

# J-001: Account Access and Recovery

## Outcome

An eligible person can create, secure, access, and recover an account without exposing account existence or weakening protections.

## States

`anonymous` → `registration_started` → `verification_pending` → `active` → `restricted` → `closed`. Recovery creates a time-limited challenge, never a permanent bypass of stronger authentication.

## Acceptance rules

- Registration reveals no account-existence information beyond the chosen channel’s safe response.
- Credential changes require recent authentication and notify existing trusted channels.
- Session lists show device/session metadata, allow revocation, and exclude precise location by default.
- Repeated failures trigger proportionate rate limits and risk review, not permanent silent lockout.
- Closed accounts follow the retention and deletion workflow.
