# Entity: Profile

**Owner:** Profile. Profile is the stable aggregate root for an account’s owned presentation. It stores account reference, lifecycle state, active revision reference, visibility policy reference, policy acknowledgements, and timestamps.

One account has at most the policy-approved number of profiles. Publication requires a valid active revision, eligibility assertions where required, and a visibility policy. Archived profiles are absent from public projections.
