---
status: draft
owner: architecture
last_reviewed: 2026-07-16
---

# System Context

ESEP is a web and API platform serving participants, operators, and approved third-party providers. A boundary service authenticates requests; domain services own business operations; asynchronous processing handles notifications, analytics, and long-running review work.

```mermaid
flowchart LR
  U["Participants"] --> W["Web / API edge"]
  O["Operators"] --> W
  W --> I["Identity & access"]
  W --> D["Domain services"]
  D --> DB[("Operational data")]
  D --> E["Event stream"]
  E --> N["Notifications / analytics / review"]
  D --> X["Approved providers"]
```

Providers receive only the minimum data required for their contractual purpose. Every integration has an owner, failure mode, and revocation path.
