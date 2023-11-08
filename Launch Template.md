#Scaling 
Specifies all needed settings to build out an [[Elastic Compute Cloud|EC2 Instance]].
You can use [[Launch Template]] instead of clicking through a [[Elastic Compute Cloud|EC2]] wizard all the time.
### Templates vs Configurations
#### Templates
* Capable of leveraging all [[EC2 Auto-Scaling]] features
* Supports [[Versioning]]
* More granularity
* Can include [[Network|Networking]]
* Recommended
#### Configurations
* Only certain [[EC2 Auto-Scaling]] features available
* Immutable
* Limited configuration options
* Try to avoid them
* Do not contain [[Network|Networking]]
### User Data
[[User Data]] is included in the template or configuration.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/ae24b78a-7d61-4210-a0ae-15bb50cc4b1d/28986666-326e-477f-b15b-2d232e4f3014/watch