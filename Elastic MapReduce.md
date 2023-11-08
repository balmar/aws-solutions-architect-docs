---
aliases:
  - EMR
  - Amazon EMR
---
#BigData

An [[AWS]] service to help with [[Extract Transform Load|ETL]] processing.
A managed, [[Big Data]] platform that allows you to process vast amounts of data using tools such as [[Spark]], [[Hive]], [[HBase]], [[Flink]], [[Hudi]], [[Presto]].
### EMR Storage
* [[Hadoop Distributed File System]]
* [[EMR File System]]
* Local File System
### [[Cluster Placement Group|Clusters]] and nodes
Node is an [[Elastic Compute Cloud|EC2 Instance]], [[Cluster Placement Group|Cluster]] is a group of Nodes
#### Primary node
Manages the cluster.
Coordinates distribution of data and tasks, tracks health statuses.
#### Core node
Runs tasks and stores data in [[Hadoop Distributed File System|HDFS]]. Long running!
#### Task Node
Only runs tasks with no storage of data within [[Hadoop Distributed File System|HDFS]]. Typically [[Spot EC2|Spot Instances]].
### Purchasing options
* [[On-Demand EC2|On-Demand]] - most reliable and expensive,
* [[Reserved EC2|Reserved]] - Minimum of 1 year. Great cost savings
* [[Spot EC2|Spot]] - cheapest option. Can be terminated
* [[Cluster Placement Group|Clusters]] - long running or transient.
### Related
[[Extract Transform Load|ETL]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7bcd3ba2-1d13-4c67-92c4-2e979998a4fd/468f4f42-d0e7-4d68-9c3e-c229895a2392/wat