---
aliases:
  - IAM
---
#IdentityManagement 

*IAM* allows you to manage [[AWS Account|users]] and their level of access to the AWS console. It is a global service. It is global and not affected by [[Region]] or [[Availability Zone|AZ]].

* Create [[AWS Account|users]] and grant permissions
* Create [[Group|groups]] and [[IAM Role|roles]]
* Control access to AWS resources
### Building blocks
* [[AWS Account|Users]],
* [[Group|Groups]],
* [[IAM Role|Roles]].

### Root account
It is the email address you use to log in to the [[AWS Console]].

> [!TIP] Securing the root account
> 1. Enable multi-factor auth
> 2. Create an admin group for administrators, assign appropriate permissions to it.
> 3. Create user accounts for your administrators.
> 4. Add users to the admin group.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/0c76f3e9-5288-4fe9-a588-fde7b034b4fb/2a4ba999-5d0c-4413-b200-acf81272ff18/watch