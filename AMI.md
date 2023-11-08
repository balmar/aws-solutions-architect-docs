---
aliases:
  - AMIs
  - Amazon Machine Image
---
#Computing 
Amazon Machine Image provides information required to launch an instance.
Running an instance requires to choose an [[AMI]].

> [!TIP] AMI is a blueprint for an [[Elastic Compute Cloud|EC2 Instance]]
### AMIs are based on
* [[Region]],
* [[Operating System]],
* [[32-bit or 64-bit Architecture]]
* [[Launch permissions]]
* [[Root Device Volume]]
### AMI can be backed by
* [[Elastic Block Storage|EBS]] - the instance will use [[Root Device Volume]] launched from a [[Snapshot]]
* [[Instance Storage]] - the instance will use the [[Root Device Volume]] created based on a template stored in [[Simple Storage Service|S3]].
### [[Elastic Block Storage|EBS]] vs [[Instance Storage]]
* [[Instance Storage|Instance Store]] based instances cannot be stopped, they can only be terminated, which causes loss of data
* [[Elastic Block Storage|EBS]] based instances can be stopped and you do not lose your data.
* Rebooting does not cause the data to be lost on both choices
* You can set up on the [[Elastic Compute Cloud|EC2]] configuration to keep [[Volume|EBS Volume]] on [[Elastic Compute Cloud|EC2 Instance]] termination, instead of deleting it by default.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/ab75a0e1-2c08-44c8-b056-1d69f25a4fc7/watch