---
aliases:
  - Auto-Scaling
---
#Computing #Scaling 
[[EC2 Auto-Scaling|Auto-Scaling]] group contains a collection of [[Elastic Compute Cloud|EC2 Instances]] that are treated as a collective group for purposes of [[Scaling]] and management.
### Auto Scaling Steps
1. Define [[Launch Template]]
2. Specify [[Network|Networking]] and [[Purchasing]] options
3. [[Elastic Load Balancer]] configuration
4. Set [[Scaling Policies]]
5. Set up [[Notifications]] using [[SNS]]
### Restrictions
#### Minimum
Lowest number of [[Elastic Compute Cloud|EC2 Instances]] you'll ever have online.
#### Maximum
Highest number of [[Elastic Compute Cloud|EC2 Instances]] you'll have.
#### Desired
How many [[Elastic Compute Cloud|Instances]] do you need right now?
### Lifecycle Hooks
You can perform a custom action on instances, when a certain lifecycle event happens.
It can wait for up to 2 hours.
![[Pasted image 20231106162630.png]]
### Step scaling
You can set up thresholds to respond accordingly 
### Instance Warm-Up
After provisioning new [[Elastic Compute Cloud|EC2 Instances]], they are not immediately registered in [[Elastic Load Balancer|ELB]]. Instead, they are put into a Warm-Up period and only after it finishes, they start receiving traffic. This prevents [[Elastic Load Balancer|ELB]] from falsely alarming about the [[Elastic Compute Cloud|Instances]] failing [[Health Checks]].
### Cooldown
Pauses [[EC2 Auto-Scaling|Auto-Scaling]] for a set amount of time. This prevents from premature termination of required resources.
### Avoid Thrashing
Add [[Elastic Compute Cloud|Instances]] quickly, terminate them slowly.
### Scaling Types
#### Reactive Scaling
The [[Scaling]] works in response to the incoming traffic.
#### Scheduled Scaling
If you have a predictive workload, you can scale up or down in advance the anticipated traffic.
#### Predictive Scaling
[[AWS]] uses [[Machine Learning]] to predict when it needs to scale. It reevaluates every 24 hours for the next 48h.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/ae24b78a-7d61-4210-a0ae-15bb50cc4b1d/80eacf6a-ed06-4f6c-9922-5810f8990db8/watch