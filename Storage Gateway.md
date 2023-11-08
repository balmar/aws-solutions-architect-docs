#Migration 

It is a service which runs on a VM on-premise.
### File Gateway
* [[Network File System|NFS]] or [[Server Message Block]] mount for caching local files
* Keep a local copy of recently used files
* *Extends on-prem storage*
* Helps with migrations to AWS
### Volume Gateway
* Backup drives
* [[Internet Small Computer System Interface]] mount
* Cached or stored mode
* Create [[Elastic Block Storage|EBS]] snapshots
### Tape Gateway
* Replace physical tapes meant for backups
* Doesn't change current workflow

> [!TIP] *Storage Gateway* is Hybrid Storage
> Pick it, if they mention a solution for data migration.
> Remember to choose
### Exam tips
* Know the general use case for *Storage Gateway* type
* When out of space - think *Storage Gateway*
* Have a high-level knowledge of Tape Gateway
### Related
[[AWS DataSync]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/1c7cb260-b6d6-4daf-9a0e-1ce05c4d7426/190fc1b9-cfd9-4c0b-9b97-1ec4248c8138/watch


[^3]: iSCSI - [internet Small Computer System Interface](https://www.techtarget.com/searchstorage/definition/iSCSI) (disk connection protocol dedicated for servers)