---
aliases:
  - NLB
---
#Network 
It operates on [[OSI Model|Layer 4]].
It can handle millions of requests per second.
### How does it work?
On connection request it selects a target from target group for the default rule.
Then it attempts to open a [[TCP]] connection on selected port.
### Listeners
A listener waits for connection requests from clients using the protocol and port you configure.
Then the request is forwarded to the target group. There are no rules as with [[Application Load Balancer]].
### Protocols
[[TCP]], [[TLS]], [[UDP]], [[TCP_UDP]]
### Ports
1-65535
### Use cases
Best fit for load balancing of [[TCP]] traffic where extreme performance is required.

> [!TIP] Network balancer can decrypt traffic
> But it requires to install the certificate.
### Related
[[Application Load Balancer]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/f4200e81-a7e0-4ffc-946f-f80ca08c038e/5e6b9bbd-66