---
aliases:
  - Bucket
  - S3 Buckets
  - Buckets
---
#S3 #Storage 

A container for keeping data in [[Simple Storage Service|S3]].

> [!INFO] Bucket needs to have a universally unique name.

> [!INFO] Buckets are private by default
> If you need to make them public, use [[Bucket Policy]]
### Example URLs
```
https://bucket-name.s3.Region.amazonaws.com/key-name
https://acloudguru.s3.us-east-1.amazonaws.com/Ralphie.jpg
```
### Uploading files
After a successful upload you will get *HTTP 200* code.
### S3 object properties
[[S3 Object]]
### Static website using S3
[[How to host a static website on S3]]
### Related
[[Simple Storage Service|S3]]
[[Bucket Policy]]
[[Access Control List|ACLs]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/c2b00f9f-aeab-4a81-bb98-1f87860