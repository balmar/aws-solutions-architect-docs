---
aliases:
  - Aurora
  - Aurora MySQL
  - Aurora PostgreSQL
---
#Databases 
Amazon [[Relational Database Service|RDS]] engine compatible with either [[MySQL]] and [[PostgreSQL]].
It is fast, highly-available, simple and cost-effective.

It is up to *5x faster* than [[MySQL]] and *3x* than [[PostgreSQL]].

Starts with 10GB and scales in *10GB* increments up to 128TB.
Compute resources can scale up to *96 vCPUs* and *768GB* memory.
### Scaling
* It is designed to transparently handle the loss of up to 2 copies of data without affecting database write availability and up to 3 copies without affecting read availability
* [[Amazon Aurora|Aurora]] is also self-healing. Data blocks and disks are continuously scanned for errors and repaired automatically
### Aurora Replicas
#### Aurora Replicas
Up to 15 read replicas with [[Amazon Aurora|Aurora]]
#### MySQL Replicas
Up to 5 read replicas with [[Aurora MySQL]]
#### PostgreSQL Replicas
Up to 5 read replicas with [[Amazon Aurora|Aurora PostgreSQL]]
### Backups
* Automated backups are always enabled.
* Backuping does not impact database performance.
* You can also take snapshots with [[Amazon Aurora|Aurora]] this also does not impact performance.
* The snapshots can be shared between [[AWS Account|AWS Accounts]].
### Aurora Serverless
On-demand, auto-scaling configuration for the [[Amazon Aurora|Aurora MySQL]] and [[Amazon Aurora|Aurora PostgreSQL]]. 
* Aurora Serverless Db cluster automatically starts up, shuts down
* Scales capacity up or down based on an app needs
#### Use cases
* Relatively simple, cost-effective option for infrequent intermittent or unpredictable workloads

### Tips
* 2 copies of your data are contained in each [[Availability Zone|AZ]], with a minimum of 3 [[Availability Zone|AZs]]. That makes at least 6 copies of your data.
* You can share [[Amazon Aurora|Aurora]] snapshots with other [[AWS Account|AWS Accounts]],
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/ceb2f84d-2f82-4d81-8e1e-7c93112e334f/watch