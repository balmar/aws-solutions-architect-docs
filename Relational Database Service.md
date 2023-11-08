---
aliases:
  - Amazon RDS
  - RDS
  - Amazon Relational Database Service
---
#Storage #Databases
A service that allows for managing of a [[Relational Database]].
### Relational databases building blocks
#### Tables
A [[Excel]]-like matrix containing data
#### Rows
Each table contains data in form of rows.
Single row consist of multiple values based on columns.
#### Columns
Column describes a single piece of data for the given row in a given table. It has a type, constraints or references.
### Examples
[[Microsoft SQL Server]]
[[PostgreSQL]]
[[Oracle RDS]]
[[MariaDB]]
[[MySQL]]
[[Amazon Aurora]]
### Benefits
* Up and running in minutes
* [[Multi-AZ RDS]]
* [[Failover capability]]
* Automated backups
### When to use
[[Online Transaction Processing]]
### Scaling [[RDS]] Database
#### [[Vertical Scaling]]
Add or take away additional computing power / memory
#### Scaling storage
You can add more storage to a database, but you *cannot* take any away.
Scale storage wisely.
#### [[Read Replica|Read Replicas]]
Add read replicas to help handle read-heavy traffic.
### [[Aurora Serverless]]
Outsource [[Scaling]] of your [[Relational Database Service|RDS]] to [[AWS]].
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/2647fb64-33d4-41db-b838-d3a495932c7b/watch