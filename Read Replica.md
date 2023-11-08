---
aliases:
  - Read Replicas
---
Read-only copy of your database. Significantly increases performance in read-heavy traffic scenarios.

* [[Read Replica]] can be cross-[[Availability Zone|AZ]] or cross-[[Region]],
* Not used for [[Disaster Recovery]]. For that case use [[Multi-AZ RDS]],
* Each [[Read Replica]] has their own [[DNS Endpoint]],
* [[Read Replica]] can be promoted to be its own database (this breaks the replication),
* Multiple [[Read Replica|Read Replicas]] are supported,
* Require automatic backups to be enabled in [[Relational Database Service|RDS]]

### Related
[[Relational Database Service|RDS]]
[[Multi-AZ RDS]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/0497544f-552c-4985-adb6-e1cb46d5243f/watch