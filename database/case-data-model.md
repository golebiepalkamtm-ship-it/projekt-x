# Case Data Model

Trust & Safety owns `Report`, `Case`, `EvidenceReference`, `CaseAssignment`, `Decision`, `EnforcementAction`, and `Appeal`. References preserve source and access policy without duplicating restricted raw content.

Cases retain a policy-version snapshot and decision trail. Enforcement actions are scoped to a subject and capability, have effective/expiry times, and emit events so every affected domain enforces them consistently.
