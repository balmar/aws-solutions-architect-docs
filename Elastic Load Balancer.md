---
aliases:
  - ELB
  - ELBs
  - Elastic Load Balancers
---
Automatically distributes incoming traffic across multiple targets, usually [[Elastic Compute Cloud|EC2 Instances]]. This can be done across multiple [[Availability Zone|AZs]].
### Types of load balancer
#### [[Application Load Balancer]]
**Intelligent Load Balancer**
Best suited for load balancing of [[HTTP]] and [[HTTP|HTTPS]].
They operate on [[OSI Model|Layer 7]] and are application aware.
#### [[Network Load Balancer]]
**Performance Load Balancer**
Capable of handling millions of requests per second with ultra-low latencies.
Operates at a connection level ([[OSI Model|Layer 4]]).
#### Gateway Load Balancer
**For Inline Virtual Appliance Load Balancing**
Use it when deploying inline virtual appliances, where network traffic is not destined for the Gateway Load Balancer itself.
Operates on [[OSI Model|Layer 3]].
#### [[Classic Load Balancer]]
**Classic/Test/Dev Load Balancer**
Legacy load balancers.
You can load [[HTTP]] / [[HTTPS]] apps using [[OSI Model|Layer 7]] specific features like `X-Forwarded` and [[Sticky Sessions]].
### Health Checks
If [[Health Checks]] determine that the service is unhealthy, its status will be `OutOfService`. The [[Elastic Load Balancer|ELB]] performs [[Health Checks]] on all registered [[Elastic Compute Cloud|Instances]] no matter if they are healthy or not.
[[Elastic Load Balancer]] only routes traffic to the `Healthy` [[Elastic Compute Cloud|Instances]].
### Deregistration Delay
The delay allows load balancers to keep existing connections after the [[Elastic Compute Cloud|EC2 Instances]] become unhealthy. This allows users to finish the in-flight requests made to them.
If you want Load Balancer to immediately close all connections to unhealthy/deregistered [[Elastic Compute Cloud|Instances]], disable *Deregistration Delay*.
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/f4200e81-a7e0-4ffc-946f-f80ca08c038e/f4906d2f-110b-4a89-8c8b-204978a1f9e4/watch      