---
aliases:
  - EBS
---
#Storage #Computing 
Storage volumes/disks you can attach to [[Elastic Compute Cloud|EC2 Instances]].
The data is spread across multiple devices to protect against hardware failures.

* Designed for production workloads
* Highly available
* Scalable (with no downtime or performance impact)
### Volume types
#### SSD
[[General Purpose SSD|General Purpose (gp2)]]
[[General Purpose SSD|General Purpose (gp3)]]
[[Provisioned IOPS SSD|Provisioned IOPS (io1)]]
[[Provisioned IOPS SSD|Provisioned IOPS (io2)]]
#### HDD
[[Throughput Optimized HDD]]
[[Cold HDD]]

### IOPS vs Throughput
[[IOPS]] is a metric for quick transactions, low latency apps. It measures how fast can you do the following reads and writes.
[[Throughput]] is a metric for large files and datasets. It measures how fast you can transfer given amount of data measured in bytes.

> [!TIP] Need big amount of IOPS?
> Choose either [[Provisioned IOPS SSD|io1]] or [[Provisioned IOPS SSD|io2]]

> [!TIP] Need to deal with big amount of data?
> Choose [[Throughput Optimized HDD|st1]].
### What happens to the [[Volume|EBS Volume]] when [[Elastic Compute Cloud|EC2 Instance]] stops or terminates
#### On stop
The [[Root Device Volume]] will persist until the [[Elastic Compute Cloud|EC2 Instance]] is started again.
#### On termination
The [[Root Device Volume]] will be terminated as well by default.
You can prevent it from termination by setting `DeleteOnTermination` attribute to *False*.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/9448f19a-5101-4b67-a701-a6ed6e93beb6/3f0f56f3-9c43-4301-9e26-46ad7e4e1a76/watch