---
aliases:
  - Placement Group
  - Placement Groups
---
#Computing 
The way of grouping your [[Elastic Compute Cloud|EC2 Instances]] within a single [[Availability Zone]].
### Types of placement groups
[[Cluster Placement Group|Cluster]] - when you need extremely low latency and high throughput.
[[Spread Placement Group|Spread]] - when you want to ensure that no 2 critical instances share a physical device.
[[Partition Placement Group|Partition]] - when you want to ensure, that no 2 groups (partitions) of critical instances share a physical device.
### Tips
* [[Cluster Placement Group|Cluster]] will always be within a single [[Availability Zone|AZ]], but [[Spread Placement Group|Spread]] and [[Partition Placement Group|Partition]] can span over multiple [[Availability Zone|AZs]].
* Only certain types of instances can be put in a [[EC2 Placement Groups]],
* It is recommended to put instances from the same computing family into [[Cluster Placement Group|Cluster]]
* [[EC2 Placement Groups|Placement Groups]] cannot be merged together
* An existing [[Elastic Compute Cloud|EC2 Instance]] can be moved into a [[EC2 Placement Groups|Placement Group]]. It needs to be in stopped state.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/576aa758-3c6f-4aad-a949-f7cb777e8c0f/watch