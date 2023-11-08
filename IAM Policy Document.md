---
aliases:
  - IAM Policy
  - IAM Policies
---
#IdentityManagement 

They determine what users can and cannot do.
You can assign a *Policy Document* to [[Group]], [[AWS Account|Users]], [[IAM Role|Roles]].

They are in the JSON format.
### Example
```
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Effect": "Allow",
			"Action": "*",
			"Resource": "*"
		}
	]
}
```
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/0c76f3e9-5288-4fe9-a588-fde7b034b4fb/0a06994f-a47d-4be5-ba31-c4a721026a5c/watch