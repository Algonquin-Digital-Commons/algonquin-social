# Commons Social Fabric

Federated social and publishing ecosystem built around ActivityPub. It owns
actors, inbox/outbox processing, federation, moderation, search, notifications,
and the user-facing Social, Photos, Video, Communities, and Blogs experiences.
Each institution operates its own sovereign actor domains, moderation, peer
policy, retention, and incident authority.

## Ecosystem dependencies

Commons Social Fabric depends on Commons Cloud Fabric for identity brokering, policy, events, secrets,
storage abstractions, and observability. It owns every external ActivityPub
boundary. Media processing and AI enrichment are optional asynchronous
capabilities; federation and ordinary publishing must remain available without
them. Public federated identity stays distinct from institutional identity unless
a person explicitly links the accounts under policy.

- [Consolidated ecosystem architecture](../psdc-architecture/docs/architecture/Consolidated-Ecosystem-Architecture.md)
- [Dependency contract](../psdc-architecture/docs/architecture/Ecosystem-Dependency-Contract.md)
- [Cross-pollination model](../psdc-architecture/docs/architecture/Cross-Pollination-and-Shared-Capabilities.md)
- [Open-source-only policy](../psdc-architecture/docs/vision/11-Open-Source-Only-Policy.md)
- [Commons architecture](../psdc-architecture/docs/vision/constitutional/Post-Secondary-Digital-Commons-Architecture.md)
- [Federated social governance policy](../psdc-architecture/docs/fediverse/Federated-Social-Governance-Policy.md)

## Layout

- `apps/` — social, photos, video, communities, blogs, and administration
- `services/` — ActivityPub gateway, actors, inbox/outbox, federation, moderation,
  media proxy, search, notifications, and spatial support
- `contracts/` — protocol and spatial integration definitions
- `connectors/` — Commons Cloud Fabric, AI, compute, and media integrations
- `policies/` — federation, moderation, privacy, and retention controls
