# Test Pyramid and Ownership

| Layer | Protects | Owner |
|---|---|---|
| Domain tests | rules, invariants, state transitions | domain team |
| Contract tests | APIs, events, providers | producing and consuming teams |
| Integration tests | persistence, authorization, queues | service team |
| Journey tests | critical user outcomes | product and engineering |
| Exploratory and accessibility tests | real-world gaps | quality and design |
| Security tests | abuse and control failures | security with service team |

Coverage is not a quality metric on its own. Tests must target risk and meaningful behavior.
