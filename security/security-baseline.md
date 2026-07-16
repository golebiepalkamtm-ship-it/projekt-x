---
status: draft
owner: security
last_reviewed: 2026-07-16
---

# Security Baseline

Security work begins with asset inventory and threat modelling. Production access uses individual identities, MFA, least privilege, short-lived credentials, and audit logs. Secrets never enter source control, client bundles, tickets, or ordinary logs.

All external input is validated at the boundary. Sensitive operations use authorization checks, rate limits, idempotency, audit events, and appropriate step-up verification. Dependencies, infrastructure, and build artifacts require provenance and vulnerability monitoring.

Security incidents follow a documented severity, containment, communication, evidence-preservation, recovery, and retrospective process.
