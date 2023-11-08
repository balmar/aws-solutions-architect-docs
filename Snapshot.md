---
aliases:
  - Snapshots
---
A point in time copy of a [[Volume]].
* [[Snapshot|Snapshots]] are incremental.
* They are stored in [[Simple Storage Service|S3]].
* The first snapshot takes usually longer to take.
> [!TIP] Consistent Snapshot
> If you need a consistent snapshot it is recommended to stop a [[Elastic Compute Cloud|EC2 Instance]]. Otherwise some data can be still stored in cache which is not copied by [[Snapshot]].

> [!TIP] Encrypted snapshots
> If you take a snapshot of an encrypted [[Volume]], the [[Snapshot]] will be automatically encrypted.

> [!TIP] Sharing snapshots
> You can share [[Snapshot]], but only in the same [[Region]]. To move to a different [[Region]], you need to copy it first. This way you can easily move existing [[Elastic Compute Cloud|EC2 Instance]].
### Related
[[Volume]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/e6099ae8-8f43-457f-af5b-7eebfa25f309/watch