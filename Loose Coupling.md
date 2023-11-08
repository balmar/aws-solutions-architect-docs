#Network #Decoupling 
A web architecture where [[Elastic Compute Cloud|Instances]] never directly reference other [[Elastic Compute Cloud|Instances]]. There is always [[Elastic Load Balancer]] between them, which has one or more [[Elastic Compute Cloud|Instances]] registered.

This way, all [[Elastic Compute Cloud|Instances]] in a group would have to break for application to stop working.

![[Pasted image 20231106201638.png]]
### Related
[[Tight Coupling]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/b936b7ef-c649-4430-a1ba-abfba6a850b0/watch