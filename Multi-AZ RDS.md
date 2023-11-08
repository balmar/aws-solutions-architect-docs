#Databases 

[[Relational Database Service|RDS]] creates an exact copy of your production database in another [[Availability Zone]].
[[AWS]] handles the replication for you.
It is meant for [[Disaster Recovery]], not for improving performance.
### Supported database types
* [[Amazon Aurora]] - always [[Multi-AZ RDS]]
* [[MySQL]]
* [[MariaDB]]
* [[Oracle RDS]]
* [[PostgreSQL]]
### Use case
Failover database - move the traffic to a replicated copy once the main database is down. [[Relational Database Service|RDS]] will automatically do that for you.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/2647fb64-33d4-41db-b838-d3a495932c7b/watch