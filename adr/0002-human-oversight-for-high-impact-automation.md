---
status: accepted
date: 2026-07-16
deciders: [product, safety, architecture]
---

# ADR-0002: Keep human oversight for high-impact automation

Automated systems may rank, recommend, detect abuse, or prioritise work. They may not make irreversible high-impact decisions about access, safety enforcement, eligibility, or funds without a defined human review, appeal, and audit path.

This reduces unsafe automation risk and requires the platform to preserve evidence, model/version context, operator actions, and reversal mechanisms.
