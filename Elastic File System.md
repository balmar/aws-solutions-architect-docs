---
aliases:
  - EFS
---
#Storage #EFS 
Managed [[Network File System]].
* It can be mounted on multiple [[Elastic Compute Cloud|EC2 Instances]],
* [[Elastic File System|EFS]] can be attached to [[Elastic Compute Cloud|EC2 Instances]] in multiple [[Availability Zone|AZs]]
* Uses [[NFSv4 protocol]]
* Compatible with [[Operating System|Linux]]-based [[AMI|AMIs]]
* Highly available, but costly
* [[Encryption at rest]] using [[AWS Key Management Service|KMS]]
* It scales automatically
* Pay per use

> [!TIP] When they ask you for highly scalable shared storage using [[Network File System|NFS]]

### EFS Performance
* 1000s of concurrent connections
* 10Gbps [[Throughput]]
* Scales to Petabytes
### Performance controlling
* *General purpose* - web servers, [[Content Management Systems|CMS]] etc.
* *Max I/O* - [[Big Data]], Media processing
### Storage tiers
* *Standard* - frequently accessed files
* *Infrequently accessed* - a bit cheaper infrequently accessed files

### Use cases
* Great fit for [[Content Management Systems]], because you can easily share content between [[Elastic Compute Cloud|EC2 Instances]].
* Also works well for web servers.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/64caf5dd-0e62-426c-a088-91f7bf33829a/watch