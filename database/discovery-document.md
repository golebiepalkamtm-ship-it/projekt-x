# Entity: Discovery Document

**Owner:** Discovery. A document is a denormalized, minimised projection of eligible public profile data. It contains profile reference, projection version, filterable approved fields, ranking features, visibility scope, and index timestamps.

The document is rebuilt from events, not edited by other domains. Restricted or deleted profiles are removed with a high-priority event and periodic reconciliation. Indexes avoid private fields and sensitive inferred attributes.
