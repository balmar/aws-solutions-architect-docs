#Computing 
Allows you to run [[Batch Workloads]] on [[Elastic Compute Cloud|EC2]], [[Elastic Container Service|ECS]] or [[Amazon Fargate]].
### Main features
* Simplifies configurating and managing of infrastructure needed for [[Compute|Computing]],
* Capable of auto-provisioning and [[EC2 Auto-Scaling|Auto-Scaling]] based on number of jobs
* No installation of batch software needed

### [[Amazon Fargate]] or [[Elastic Compute Cloud|EC2]] for [[Compute Environment|Compute Environments]]?
#### Choose Fargate 
* when you need Fast start times (<30s).
* (Recommended for most workloads)
#### Choose EC2
* when you need more control,
* high levels of concurrency,
* access to [[Linux Parameters]]
### [[AWS Batch]] or [[Lambda]]?
Depends on your case...
#### Time limits
[[Lambda]] can run for max 15 mins
#### Disk Space
[[Lambda]] has limited disk space and [[Elastic File System|EFS]] requires [[Virtual Private Cloud|VPC]]
#### Runtime Limitations
[[Lambda]] is [[Serverless]], but has limited runtimes.
#### Batch Runtimes
[[AWS Batch]] uses [[Docker]], so any runtime can be used.
### Managed or Unmanaged [[Compute Environment|Compute Environments]]
#### Managed
* [AWS]] manages capacity and [[Elastic Compute Cloud|Instance]] types.
* [[Compute]] specs are defined on environment creation.
* [[Elastic Container Service|ECS]] instances are launched into [[Virtual Private Cloud|VPC]] [[Subnet|Subnets]].
* Most recent and approved [[AMI]] for [[Elastic Container Service|ECS]] by default
* You can use your own [[AMI]]
* Leverage [[Amazon Fargate]], [[Fargate Spot]], [[Spot EC2|Spot Instances]]
#### Unmanaged
* You manage everything,
* [[AMI]] must meet specs,
* Less common,
* Good for complex or specific requirements
### Related
[[Batch Job]]
[[Job Queue]]
[[Job Definition]]
[[Compute Environment]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/7d66d448-e9cc-40f3-9918-0cad5eff19fd/watch