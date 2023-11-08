#IdentityManagement 

An IAM user group is a collection of IAM users. User groups let you specify permissions for multiple users, which can make it easier to manage the permissions for those users.
### Main features
- A user group can contain many users, and a user can belong to multiple user groups.
- User groups can't be nested; they can contain only users, not other user groups.
- There is no default user group that automatically includes all users in the AWS account. If you want to have a user group like that, you must create it and assign each new user to it.
- The number and size of IAM resources in an AWS account, such as the number of groups, and the number of groups that a user can be a member of, are limited. For more information, see [IAM and AWS STS quotas](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_iam-quotas.html).
### Source
https://docs.aws.amazon.com/IAM/latest/UserGuide/id_groups.html