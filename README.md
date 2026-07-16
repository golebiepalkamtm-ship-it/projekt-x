# ESEP

ESEP is a documentation-first blueprint for an Enterprise Social Entertainment Platform. The repository is its operating system: decisions, product behavior, architecture, data design, delivery practices, and implementation contracts live here before code.

## Current state

The project is in **Foundation**. The documents in this first package establish how we make and retain decisions; they do not claim that the product or its legal model has been approved.

## Navigation

- [Project memory](docs/project-memory.md) — durable decision log.
- [Enterprise blueprint](docs/enterprise-blueprint.md) — platform intent and boundaries.
- [Vision 2.0](docs/vision-2.0.md) — canonical platform direction.
- [Module catalog](product/module-catalog.md) — enterprise capability inventory.
- [Product principles](product/product-principles.md) — rules for user-facing design.
- [Architecture overview](architecture/system-context.md) — system boundaries.
- [Data principles](database/data-principles.md) — database design contract.
- [AI Operating Manual](ai/ai-operating-manual.md) — required coding rules.
- [AI policy](ai/ai-governance.md) — human control and model safeguards.
- [Security baseline](security/security-baseline.md) — minimum security posture.
- [Prisma schema](prisma/schema.prisma) — canonical physical data model.
- [OpenAPI](openapi/openapi.yaml) — public API-edge surface.

## Working agreement

1. A material product or technical decision receives an ADR and a Project Memory entry.
2. Specifications precede implementation. Code may not silently redefine a documented contract.
3. Open questions are explicit. Do not invent legal, payment, or policy requirements.
4. Every public API and every personal-data flow must be documented and testable.

See [CONTRIBUTING.md](CONTRIBUTING.md) for document conventions.
