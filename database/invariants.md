# Cross-domain Invariants

1. A resource has one owning domain and an opaque immutable identifier.
2. No public projection contains a field whose visibility is not explicitly public.
3. A safety restriction is enforceable at every relevant entry point, not only in the UI.
4. An operator’s sensitive action produces an immutable audit event with reason and subject.
5. Money movement is represented by balanced, immutable ledger postings.
6. Deletion requests are tracked to completion across projections, indexes, queues, and providers.
7. Events are attributable to a committed state transition or documented external observation.
