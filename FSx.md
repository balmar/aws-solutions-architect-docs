---
aliases:
  - Amazon FSx
  - FSx for Windows
  - FSx for Lustre
---
#Storage #EFS

### FSx for Windows
Fully managed native [[Operating System|Windows]] file system, so you can easily move your [[Operating System|Windows]]-based applications that require file storage to [[AWS]].
It runs on Windows Server.
#### How is it different from [[Elastic File System|EFS]]?
* It is designed for [[Operating System|Windows]], [[Elastic File System|EFS]] for [[Operating System|Linux]].
* Supports [[Active Directory|AD]] users, [[Access Control List|ACLs]], [[Distributed File System]], [[Namespaces]] and [[Replication]]
* Uses [[Operating System|Windows]] [[Server Message Block|SMB]]-based file services, [[Elastic File System|EFS]] uses [[Network File System|NFS]].
### FSx for Lustre
A fully managed file system that is optimized for compute-intensive workloads. Use cases include:
* [[High Performance Computing|HPC]],
* [[Machine Learning|ML]],
* Media data processing workflows
* Electronic design automation
* AI
With [[FSx|FSx for Lustre]] you can launch and run [[Lustre File System]] which can process massive datasets at up to hundreds of GBs per second [[Throughput]], millions of [[IOPS]], sub-ms latencies.
It can store data directly on [[Simple Storage Service|S3]].

### When to use which
* [[Elastic File System|EFS]] - distributed, highly resilient storage for [[Operating System|Linux]] instances,
* [[FSx|FSx for Windows]] - centralized storage for [[Operating System|Windows]] instances or applications such as [[SharePoint]], [[Microsoft SQL Server]], [[Microsoft Workspaces]], [[IIS Web Server]] etc.
* [[FSx|FSx for Lustre]] - high-speed, high capacity, distributed file storage. For apps with [[High Performance Computing|HPC]], [[Machine Learning|ML]], etc. 
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/3b10325c-7217-4685-a4ca-8f819a5d2db3/watch