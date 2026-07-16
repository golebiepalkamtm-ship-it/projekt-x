# Architecture Principles

1. Own data by domain; do not share tables as an integration mechanism.
2. Treat external providers as unreliable and privacy-sensitive boundaries.
3. Prefer explicit, versioned contracts over implicit framework coupling.
4. Encrypt sensitive data in transit and at rest; minimize collection first.
5. Make operational actions observable, attributable, and reversible where feasible.
6. Design for degraded operation: queues retry safely and user-visible actions have clear status.
