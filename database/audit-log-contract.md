# Audit Log Contract

Audit events record actor, role/capability, action, target reference, purpose/reason, outcome, correlation ID, time, source, and policy/version context. They do not store raw secrets or unnecessary content.

Audit storage is append-only for ordinary operators. Access is limited, monitored, and retention-controlled. A correction produces a compensating event rather than overwriting the original observation.
