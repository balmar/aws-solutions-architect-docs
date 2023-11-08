---
aliases:
  - SSE
---
#S3 #Storage 

* *SSE-S3*: S3 managed keys, using AES 256-bit encryption
* *SSE-KMS*: AWS Key Management Service-managed keys
* *SSE-C*: Customer-provided keys

### Enforcing [[Server-Side Encryption|SSE]]
To enforce *SSE* add `x-amz-server-side-encryption` header to the PUT request. Then it is possible to use either `AES-256` or `aws:kms` 
### Related
[[Client-Side Encryption]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/203ccc3c-bdb8-44fd-b818-ed2a0f8b9e1f/