---
aliases:
  - Amazon DynamoDB
---
#Databases 

This is a fast and flexible [[NoSQL Database]] service.
* It provides consistent, low latency [[NoSQL Storage]].
* Fully managed database.
* Supports both document and key-value data models,
* Great fit for mobile, web, gaming, ad-tech, IoT and other applications,
* It is stored on a [[SSD Storage]]
* Spread across 3 geographically distinct [[Data Centers]]
### Read consistency
[[Eventually Consistent Reads]] (default)
[[Strongly Consistent Reads]]
Transactional reads
### Transactions
[[DynamoDB]] supports transactions, which follow the [[ACID Principle]]. This means the change happens whole, or not at all.
### Backups
See [[DynamoDB Backups]]
### Related
[[DynamoDB Accelerator]]
### Streams
[[DynbamoDB Streams]]
### Global Tables
[[DynamoDB Global Tables]]
### Scaling models
#### Provisioned [[Scaling]]
* When to use? - Generally predictable workload
* Effort? - Review past usage to set upper and lower scaling bounds
* Cos? - Most cost-effective
#### On-Demand [[Scaling]]
* When to use? - Sporadic workload
* Effort? - Simply select an option
* Cost? - Pay small amount of money per read and write. Less cost-effective
### Scaling units
[[Read Capacity Unit]]
[[Write Capacity Unit]]
### Related
[[NoSQL Database]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/1fd3d060-62c9-4894-b27e-b794c5ed1876/watch                