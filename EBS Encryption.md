#Security #Storage #Encryption 
[[Elastic Block Storage|EBS]] encrypts your volume using [[AES-256 algorithm]].
[[EBS Encryption]] uses [[AWS Key Management Service|AWS KMS]] [[Custom Master Keys]] to encrypt [[Volume|Volumes]] and [[Snapshot|Snapshots]].

### What happens after encrypting [[Volume|EBS Volume]]?
* Data at rest is encrypted inside the volume,
* All data in flight moving between the instance and the volume is encrypted
* All [[Snapshot|Snapshots]] are encrypted,
* All [[Volume|Volumes]] created from the [[Snapshot]] are encrypted.
### Features
* It is handled transparently without you doing anything,
* It has a minimal impact on latency
* Copying an unencrypted snapshot supports encryption
* [[Snapshot]] of an encrypted [[Volume]] will be encrypted
* You can encrypt [[Root Device Volume|Root Device Volumes]] upon creation
### Related
[[How to encrypt existing EBS Volumes]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/f556c3a8-758d-4b1d-87ae-9f8b3644495b/watch