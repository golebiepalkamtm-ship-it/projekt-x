# Platform Capability Map

```mermaid
flowchart TB
  F["Foundation: identity, policy, consent, trust, wallet, notification, search, analytics"]
  F --> S["Social Network"]
  F --> D["Dating Engine"]
  F --> P["Professional Directory"]
  F --> L["Live Streaming"]
  F --> M["Messaging"]
  F --> C["Creator & Marketplace"]
  F --> A["AI Platform"]
  F --> O["Administration & Operations"]
```

Foundation capabilities expose stable contracts. Experience modules may consume them but never own another module’s records or bypass safety, consent, jurisdiction, or payment controls.
