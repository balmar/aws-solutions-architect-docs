---
aliases:
  - Spot Instance
  - Spot Instances
---
#Computing 
Use your [[Elastic Compute Cloud|EC2 Instance]] based on the current demand in the [[Region]].
It can be purchased at a price of up to 90% discount comparing to [[On-Demand EC2]].
### When to use
* Stateless, fault-tolerant or flexible applications
### Best for
* Processes that can be terminated early,
* Urgent need for a large amounts of additional computing capacity,
* Cost-sensitive apps, which make sense when the price is low,
* Apps that have flexible start and end times
### Bad for
* Persistent workloads
* Critical jobs
* Databases
### Examples
* Big data
* Containerized workloads
* Image and media rendering
* CI/CD
* [[High Performance Computing|HPC]]
* Test and development
### Spot price
To use [[Spot EC2|Spot Instance]] you must decide on your maximum price.
The [[Elastic Compute Cloud|EC2 Instance]] will be provisioned so long as the Spot price is *BELOW* your chosen max price.

### Terminating [[Spot EC2|Spot Instance]]

![[Pasted image 20231104150831.png]]
![[Pasted image 20231104150906.png]]
> [!WARN] Terminating your [[Spot EC2|Spot Instance]] may result in its relaunching itself
> You need to cancel your persistent spot request to stop a [[Spot EC2|Spot Instance]] for good, because the Spot Request will try to accommodate to your predefined max price and desired number of instances.

### How to block [[Spot EC2|Spot Instance]] from terminating?
Use [[Spot Block]].
### Related
[[On-Demand EC2]]
[[Reserved EC2]]
[[Spot EC2]]
[[Dedicated EC2]]
[[Elastic Compute Cloud|EC2]]
[[Spot Fleet]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/071760f1-41ce-41c9-a8e2-ebff47be169c/watch