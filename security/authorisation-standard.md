# Authorisation Standard

Every request checks authenticated actor, declared capability, target resource, tenant/audience scope, resource state, and purpose where sensitive. The server enforces authorisation independently from UI visibility.

Default deny applies. Privileged access is role- and time-bounded, reviewed regularly, and produces audit events. Tests include horizontal and vertical privilege-escalation attempts.
