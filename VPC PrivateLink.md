#Network 
It creates a private connection between tens, hundreds, thousands of [[Virtual Private Cloud|VPC]]. Can connect to [[On-premise]] [[Virtual Private Cloud|VPC]].
* Doesn't require [[VPC Peering]], no [[Route Table|Route Tables]], [[NAT Gateway]], [[Internet Gateway]], etc. 
* Requires [[Network Load Balancer]] on the service [[Virtual Private Cloud|VPC]] and [[Elastic Network Interface]] on the customer [[Virtual Private Cloud|VPC]]
* [[How to share an application across VPCs]]

> [!TIP] Fits the questions about peering tens, hundreds or thousands of [[Virtual Private Cloud|VPC]]
### Use cases
* Securely access [[AWS]] services
* Maintain regulatory compliance by transferring data via secure connection,
* Migrate to hybrid cloud
* Deliver [[SaaS]] services
### Diagram
![[Pasted image 20231105155058.png]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/e895e0dc-ee49-4a4e-9252-6018c96def38/b36018c7-e208-4f2d-84fb-1623ba3b8310/watch