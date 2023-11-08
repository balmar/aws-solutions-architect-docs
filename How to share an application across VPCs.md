Either:
### Open the VPC up to the Internet
* It comes with some security considerations, as everything will be publicly accessible
* A lot more to manage
### [[VPC Peering]]
* One has to create and manage many different peering relationships
* The whole network will be accessible. This may not be the best thing if you have multiple applications.
### [[VPC PrivateLink]]
* It is designed to handle tens, hundreds, thousands of [[Virtual Private Cloud|VPC]],
* Doesn't require [[VPC Peering]], which means no [[Route Table|Route Tables]], [[NAT Gateway]], [[Internet Gateway]]
* Requires [[Network Load Balancer]] on the service [[Virtual Private Cloud|VPC]] and an [[Elastic Network Interface]] on the customer [[Virtual Private Cloud|VPC]].
![[Pasted image 20231105155043.png]]