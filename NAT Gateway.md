---
aliases:
  - Network Address Translation
---
#VPC #Network 
[[NAT Gateway|Network Address Translation]] gateway can serve as a proxy for [[Elastic Compute Cloud|Instances]] inside the private [[Subnet|Subnets]], allowing them to access internet, however preventing anyone from the internet to initiate a connection with those [[Elastic Compute Cloud|Instances]].

If deployed, it becomes a part of [[Subnet]].
### Main Features
* Redundant inside the [[Availability Zone|AZ]]
* Starts at 5 Gbps and scales up to 45 Gbps
* No need to patch
* Not associated with [[Security Group|Security Groups]]
* Auto-assigned a public [[IP Address]]
### Diagram
![[Pasted image 20231105135757.png]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/e895e0dc-ee49-4a4e-9252-6018c96def38/acbd237f-2494-4520-a912-2b29481c4038/watch