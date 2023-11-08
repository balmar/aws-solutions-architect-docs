---
aliases:
  - VPC
---
A Virtual Data Center in the [[AWS]].
* Logically isolated part of [[AWS|AWS Cloud]] where you can define your own [[Network]]
* Gives you a complete control over your [[Network|Virtual Network]]
* You can create hardware [[Virtual Private Network]]
### CIDR range
You can check which IP addresses match the provided [[CIDR]] notation in [here](https://cidr.xyz).
### Logical network division
![[Pasted image 20231105133056.png]]
### What can you do with a VPC?
* Launch instances
* Custom IP Addresses
* [[Route Table]]
* [[Internet Gateway]]
* [[Access Control List]]
* [[Network Access Control List]]
### Default VPC vs Custom VPC
#### Default VPC
* User friendly
* All [[Subnet|Subnets]] in Default [[Virtual Private Cloud|VPC]] have a route out to the internet
* Each [[Elastic Compute Cloud|EC2 Instance]] has both public and private [[IP Address]]
#### Custom VPC
* Fully customizable
* Takes time and skill to set up
### Related
[[NAT Gateway]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/e895e0dc-ee49-4a4e-9252-6018c96def38/2451d7b5-b7c5-4e72-960c-5e759c9