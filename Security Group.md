---
aliases:
  - Security Groups
  - SG
---
#Security #Network 
A virtual firewall for your [[Elastic Compute Cloud|EC2 Instance]].
* By default everything is blocked.
* To unblock access for specific ports and source [[IP Address|IPs]], you need to use [[Security Group|Security Groups]].
* The last line of defense in the [[Network]].
* You can assign up to five security groups to an instance.

> [!TIP] To let everything in use 0.0.0.0/0
> Usually it is not a good idea

> [!WARN] [[Security Group|Security Groups]] are stateful
> It means, that the responses are allowed to flow, regardless of the outbound rules.
> If some entity was able to connect via [[SSH]] to your [[Elastic Compute Cloud|Instance]], then you don't have to worry about unlocking [[SSH]] also on outbound traffic.
### Diagram
![[Pasted image 20231105135938.png]]
### Default [[Security Group|Security Groups]]
* You CAN change the rules for a Default [[Security Group|SG]]
* You CANNOT delete a Default [[Security Group|SG]]
### Related
[[Elastic Compute Cloud|EC2]]
[[Elastic Compute Cloud|EC2 Instance]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/4cd7b523-0cb7-49ae-b7ee-4089a6a83872/watch