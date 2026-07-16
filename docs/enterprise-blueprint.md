---
status: approved
owner: architecture
last_reviewed: 2026-07-16
related_adrs: [ADR-0001, ADR-0002]
supersedes_open_questions_in: [RFC-0001]
---

# Enterprise Blueprint

ESEP (working codename; product name: HEXXXO) is a modular platform for discovering, verifying, and transacting with independent adult-content creators and companionship-adjacent service providers. It replaces informal channels with verified profiles, auditable payments, and appealable trust and safety.

## Market and policy envelope

| Decision | Approved value |
|---|---|
| Initial market | Poland; launch language `pl-PL` |
| Expansion | EU/EEA one jurisdiction at a time behind a jurisdiction flag |
| Eligibility | 18+ only; passed `AGE_18_PLUS` assertion before publication |
| Permitted content | creator-controlled adult content and companionship-adjacent services, subject to policy |
| Prohibited | minors, non-consensual content, trafficking indicators, and unlicensed regulated services |
| Payments | wallet and immutable ledger, with provider settlement and platform commission |
| Verification | third-party KYC/liveness; no raw ID documents stored by the platform |
| Data controller | operating legal entity for account/payment data; verifier is processor under DPA |

Changing any row requires an ADR.

## Platform commitments

- Safety, consent, privacy, and legal compliance constrain growth features.
- Identity and trust signals are explainable, appealable, and proportionate.
- Financial, moderation, and access-control actions are auditable.
- The platform can evolve by bounded context without forcing a rewrite.

## Bounded contexts

Identity and access, profiles, discovery, trust and safety, communications, scheduling, commerce, notifications, analytics, and administration are independent ownership areas. Contexts exchange versioned events rather than write directly into each other’s data.

## Initial deployment shape

Use a modular monolith (Next.js, TypeScript, PostgreSQL) with a transactional outbox. Split services only when the criteria in `architecture/service-boundaries.md` are met. Native mobile apps and self-built live-streaming infrastructure are out of scope for v1.
