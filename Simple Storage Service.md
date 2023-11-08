---
aliases:
  - S3
---
An object based storage.
### Features
* Scalable (scales automatically)
* Durable
* Secure
* Easy to use
* [[Lifecycle management]]
* [[Object Versioning]]
* [[Server-Side Encryption]]
* [[Access Control List]]
* [[Bucket Policy|Bucket Policies]],
* Supports any file type
* Cannot be used to run an operating system or database
* Max file size is 5TB
* Unlimited storage
* S3 holds data in [[S3 Bucket]]
* S3 offers many [[S3 Tier|Tiers]] depending on your use case
* Names must be globally unique
* [[S3 Event Notifications|Event Notifications]]
### Availability
`99.95% - 99.99%` depending on [[S3 Tier]].
### Durability
`99.999999999%` (11 9's) for data stored in [[Simple Storage Service|S3]] 
### Tiers
[[S3 Tier|S3 Tiers]]
### Strong Read-After-Write Consistency
On successful write or update, the next subsequent read request will receive that object.
Even the next list operation will reflect the newest state.

### Use cases
* Your general storage
* Static website

### Related
[[S3 Bucket]]
[[S3 Tier]]
[[How to host a static website on S3]]
[[How to enable public access in S3 Bucket]]
[[S3 Performance]]
[[Amazon EventBridge]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/c2b00f9f-aeab-4a81-bb98-1f878