# Profile Data Model

Profile owns `Profile`, `ProfileRevision`, `VisibilityPolicy`, `MediaAssetReference`, and `ProfileProjection`. Revisions are immutable snapshots; the active projection points to the approved revision and is rebuilt when visibility or policy changes.

Search consumes a deliberately minimised public projection. Private fields use distinct access checks and may not enter generic analytics events or search documents.
