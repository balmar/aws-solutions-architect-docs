---
aliases:
  - Instance Store
  - Ephemeral Storage
---
#Storage 
A temporary block-level storage for [[Elastic Compute Cloud|EC2 Instance]].
The data is stored on disks physically attached to the host computer.

* The size of an [[Instance Storage|Instance Store]] and the number of available devices varies depending on the [[Elastic Compute Cloud|EC2 Instance]] types.
* The devices are named `ephemeral[0-23]`
* Pricing is included in the [[Elastic Compute Cloud|EC2 Instance]] cost.
* Stopping the machine or terminating it will purge the data on [[Instance Storage]].
* Restarting does not delete the data.
### Use cases
For data that changes frequently such as
* caches,
* buffers,
* scratch data,
* other temporary content.

### Related
[[Volume|EBS Volume]]
[[Root Device Volume]]
[[AMI]]
### Source
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/ab75a0e1-2c08-44c8-b056-1d69f25a4fc7/watch