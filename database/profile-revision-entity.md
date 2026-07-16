# Entity: Profile Revision

**Owner:** Profile. A revision is an immutable, authored snapshot of editable profile fields. It has profile reference, revision number, author, field payload classification map, validation version, submitted time, and review outcome.

Revision number is unique per profile. Draft mutations create a new revision or controlled draft update; published revisions remain immutable to preserve auditability and reproducible projections.
