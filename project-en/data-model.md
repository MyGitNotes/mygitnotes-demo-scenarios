---
title: Data model
tags: [spec, data]
status: specifying
---
# Data model

Four things to store: shops, neighbours, parcels and the messages sent about them.

```mermaid
erDiagram
    SHOP ||--o{ PARCEL : holds
    NEIGHBOUR |o--o{ PARCEL : "is addressed to"
    PARCEL ||--o{ MESSAGE : triggers
    PARCEL {
        string id
        string recipient_name
        string shelf
        string pickup_code
        string status
        datetime arrived_at
        datetime collected_at
    }
    NEIGHBOUR {
        string id
        string name
        string contact
    }
    MESSAGE {
        string id
        string channel
        datetime sent_at
    }
```

## Notes on the fields

- `status` is one of *waiting*, *collected* or *returned*.
- `pickup_code` is six digits and unique among waiting parcels in one shop.
- A neighbour is optional. A shopkeeper can check in a parcel for a name nobody has registered.

See [Pickup flow](spec-pickup-flow.md) for how these fields change.
