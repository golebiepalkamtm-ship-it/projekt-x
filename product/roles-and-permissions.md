# Roles and Permissions

Initial role names are intentionally generic until RFC-0001 is accepted.

| Role | Baseline capability | Restrictions |
|---|---|---|
| Visitor | View public, policy-permitted material | No protected data or transactions |
| Participant | Manage own profile and permitted workflows | Cannot access others’ non-public data |
| Support operator | Resolve assigned support cases | No policy override or unrestricted data export |
| Safety reviewer | Review safety cases and record decisions | Actions need reason codes and audit trail |
| Administrator | Manage platform configuration | Privileged access is time-bound and logged |

Permissions are capability-based, scoped to a resource and purpose, and evaluated server-side.
