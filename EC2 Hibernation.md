---
aliases:
  - Hibernation
---
#Computing 
When you hibernate an [[Elastic Compute Cloud|EC2 Instance]], the [[Operating System|OS]] saves the contents of [[RAM memory]] to the [[Root Device Volume]]. This way all the running processes are "hibernated" and can be unpaused at later stage.
### Starting [[Elastic Compute Cloud|EC2 Instance]] out of [[EC2 Hibernation|Hibernation]]
1) [[Root Device Volume]] is restored to its previous state,
2) [[RAM memory]] contents are reloaded,
3) The suspended processes are resumed,
4) Previously attached data volumes are reattached and the instance retains its [[Instance ID]].
### Why use [[EC2 Hibernation|Hibernation]]?
The instance boots much faster after [[EC2 Hibernation|Hibernation]], because it does not need to warm up the processes, they are restored already up and running.
### Features
* [[EC2 Hibernation|Hibernation]] preserves the [[RAM memory]] on [[Volume|EBS Volume]],
* Much faster to boot
* [[RAM memory]] must be lower than *150GB*
* Available for [[Operating System|Windows]], [[Operating System|Linux]].
* Instances can be hibernated up to *60 days*
* Available for [[On-Demand EC2|On-Demand Instances]] and [[Reserved EC2|Reserved Instances]]

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/e580ffbc-ea62-48c2-85fd-c11b8216eb0a/wat