---
aliases:
  - IAM Roles
---
#Security 
A role is an identity you can create in [[Identity and Access Management|IAM]] that has specific permissions. A role is similar to a user, as it is an [[AWS Account|AWS Identity]] with permission policies that determine what it can and cannot do in [[AWS]].
### Does assuming roles give a permanent permissions?
Access based on roles is temporary. Roles are meant to be assumed only to perform a destined task and then the role session should be closed.
### Who can use IAM Roles?
Roles can be assumed by:
* people, [[AWS Account]],
* AWS Architecture,
* System-level accounts.

> [!TIP] It is not associated with one person
> Role can be assumed by any entity who has the right permission to assume it.  
### What is the biggest advantage of roles?
Using roles provides access to resources without the use of access key IDs and secrets. This alone could help avoiding hard-coding credentials for different accounts.

> [!WARNING] Roles are a preferred security option
### Is it possible to attach or detach roles from a running [[Elastic Compute Cloud|EC2 Instance]]?
Yes. You don't have to stop the instance or terminate it. The role should be assigned instantly.

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/f3d76710-cec8-441e-a39e-df15d223091e/watch