Use *S3 Object Lock* to store objects using [[WORM model]]. It helps prevent users from deleting or modyfing [[S3 Object|S3 Objects]] or entire [[S3 Bucket]].
### Modes
#### Governance mode
Users with a specific permissions are able to delete or overwrite an object version or alter it's lock settings.

This protects objects against being deleted by most users.
#### Compliance mode
Protected [[S3 Object]] cannot be overwritten or deleted by any user, including the [[Root Account]]. The retention of an object locked in *Compliance mode* can't be changed.

Basically the *Compliance mode* ensures the [[S3 Object]] remains unchanged until the of the retention period.
### Retention period
Protects an [[S3 Object]] for a fixed amount of time. [[AWS]] stores a timestamp inside of the object version's metadata which indicates the end of the retention period.

After it expires, the object version can be overwritten or deleted unless there is also a Legal Hold on the object version.
> [!TIP] When *Object Lock* is applied to bucket, objects are not automatically protected
> If you want to automatically protect object versions that are placed in the bucket, you need to configure a default retention period.
### Legal hold
It's like an *S3 Object Lock*, but it has no retention period.
It can be placed or removed by anyone with `s3:PutObjectLegalHold` permissions.
### Related
[[4. Simple Storage Service (S3)]]
[[Glacier Vault Lock]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/a06dde7a-db30-4554-bdd3-00eb7267f63d/watch
https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lock.html
https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lock-overview.html