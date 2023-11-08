#Computing 
A collection of [[Spot EC2|Spot Instances]] and (optionaly) [[On-Demand EC2|On-Demand Instances]].

The [[Spot Fleet]] will try keep the specified target capacity of [[Spot EC2|Spot Instances]] and [[On-Demand EC2|On-Demand Instances]]. It will try to relaunch interrupted [[Spot EC2|Spot Instances]].

The [[Spot Fleet]] request is fulfilled or not based on the available capacity and the specified maximum price.

[[Elastic Compute Cloud|EC2 Instances]] can be put into a different launch pools which are described by [[Elastic Compute Cloud|EC2]] instance type, OS, [[Availability Zone|AZ]].

You can hold multiple pools in a single fleet. The [[Spot Fleet]] will choose the best way to implement depending on defined strategy.

[[Spot EC2|Spot Instances]] will not be launched if the maximum price is exceeded.
### Available strategies
#### capacityOptimized
The [[Spot EC2|Spot Instances]] will come from a pool with an optimal capacity.
#### lowestPrice
The default strategy.
The [[Spot EC2|Spot Instances]] will come from a pool with the currently lowest price.
#### diversified
[[Spot EC2|Spot Instances]] are distributed equally across all pools.
#### InstancePoolsToUseCount
You choose which pools to pull from based on the `lowestPrice` parameter.

### Related
[[Spot EC2|Spot Instance]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/548ce9b6-4c3b-4615-9806-975ac728602f/watch