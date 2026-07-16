# Row-Level Security Strategy

Row-level security is enabled for multi-tenant or owner-scoped data where the storage engine supports it. The application sets trusted request context only after authentication and server-side authorization; clients never set security context directly.

Policies separate owner self-service, audience-limited read, operator case access, and service access. Background jobs use narrowly scoped service identities. RLS policies are versioned, tested with negative cases, and reviewed alongside API authorization.
