# Entity: Account

**Owner:** Identity. **Purpose:** lifecycle of an authenticated actor.

Core attributes: opaque ID, creation time, status, status reason category, credential policy, authentication assurance level, and closure request state. Account excludes public presentation data, raw verification evidence, and financial balances.

Indexes support unique normalised login identifiers held in a protected identity store, status-based operational queries, and lifecycle review. Status updates require an actor, reason, policy context, and audit event.
