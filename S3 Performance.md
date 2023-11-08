#S3 #Storage
S3 has very low latency. The first byte usually arrives within *100-200ms* with *3500* PUT/COPY/POST/DELETE and *5500* GET/HEAD requests per second, *per prefix*.

> [!TIP] To achieve better performance, move files to separate prefixes
> eg. using 2 prefixes you can achieve 11k GET/HEAD requests per second.

### S3 Limitations with KMS
#KMS
If you are using [[Server-Side Encryption|SSE]]-[[AWS Key Management Service|KMS]] to encrypt, you must keep in mind the [[AWS Key Management Service|KMS]] limits. It is 5.5k, 10k or 30k depending on your [[Region]].

Currently there is no way to increase KMS quota.
### Multipart Uploads
* Recommended for files over 100MB
* Required for files over 5GB
* Parallelize uploads (which increases efficiency)
### S3 Byte-Range Fetches
Parallelize downloads by specifying byte ranges. This increases download speed.
### Transfer Acceleration
*Amazon S3 Transfer Acceleration* can speed up content transfers to and from [[Simple Storage Service|S3]] by as much as 50-500% for long-distance transfer of larger objects. 
Customers who have either web or mobile applications with widespread users or applications hosted far away from their S3 bucket can experience long and variable upload and download speeds over the Internet.

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/5fc81ade-c884-4ede-b3f1-f57a914cd19d/watch
https://aws.amazon.com/s3/transfer-acceleration/