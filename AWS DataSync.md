#Migration #HybridCloud 
Agent based solution for migrating on-premise storage to AWS.

* It can work with [[Network File System|NFS]] and [[Server Message Block]]
* It works over [[TLS]], so it is encrypted
* Requires a working agent on the customer's datacenter
* It does not need the agent if moving between AWS storage services within the same [[AWS Account]].

> [!TIP] When to use?
> DataSync is best used for one-time migration
### DataSync vs Storage Gateway?
|DataSync|Storage Gateway|
|----|----|
|One time migration|Hybrid On-Prem + AWS solution|

### Target locations
* [[S3 Bucket|S3]]
* [[Elastic File System|EFS]]
* [[FSx]]

> [!TIP] You need high level overview of *AWS DataSync*
> It usually is used as a distractor in the exam.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/1c7cb260-b6d6-4daf-9a0e-1ce05c4d7426/94339c41-a727-4aa2-8f88-f55e32865eb7/watch