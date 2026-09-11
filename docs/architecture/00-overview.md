# Commons Social Fabric Overview

```text
apps -> shared product services -> durable inbox/outbox
                                  -> ActivityPub gateway
                                  -> remote federation

media -> Commons Media and Spatial Fabric
AI assistance -> Commons AI Fabric
shared platform -> Commons Cloud Fabric
background work -> Commons Compute Fabric
```

Only the ActivityPub gateway communicates with remote servers. Internal products
and ecosystems publish through authenticated internal APIs and versioned events.
