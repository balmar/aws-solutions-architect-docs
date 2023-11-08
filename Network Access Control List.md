---
aliases:
  - NACL
  - NACLs
---
#Network #Security 
The first line of the [[Network]] defense. Rules defined in [[Network Access Control List|NACL]] can allow or deny inbound and outbound traffic.
* It synergies well with [[Security Group|Security Groups]]. 
* Each [[Subnet]] must be associated with a [[Network Access Control List|NACL]]. 
* If you don't specify a Custom [[Network Access Control List|NACL]], your [[Virtual Private Cloud|VPC]] comes automatically with a Default [[Network Access Control List|NACL]],
* [[Network Access Control List|NACL]] can be associated with multiple [[Subnet|Subnets]], however [[Subnet]] can only be associated with a single [[Network Access Control List|NACL]].

> [!TIP] If you want to block a specific [[IP Address]], use [[Network Access Control List|NACL]]
### Default [[Network Access Control List|NACL]]
It *allows* all inbound and outbound traffic by default.
You can modify or delete rules from the Default [[Network Access Control List|NACL]], but you cannot modify or delete the *last* rule with an asterisk _*_
### Custom [[Network Access Control List|NACL]]
It *denies* all inbound and outbound traffic by default.
You can overwrite those denies by adding rules.
### Rules
Rules say if the traffic is allowed to pass through [[Network Access Control List|NACL]] or not.
They are all numbered and resolved in an order from lowest number to the highest.
Inbound and outbound rules are separate lists and each rule can allow or deny traffic.

> [!TIP] [[Network Access Control List|NACLs]] are stateless
> Responses to allowed inbound traffic are subject to the outbound rules (and vice versa)
### Related
[[Access Control List|ACL]]
[[Network]]

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/e895e0dc-ee49-4a4e-9252-6018c96def38/1f12e64e-c257-4434-9def-a016
https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html#default-network-acl