#Network 
A Load Balancer, that works on [[HTTP]]/[[HTTPS]] (Layer 7).
It evaluates the listener rules and then selects a target for action.
### Listener
A listener checks for connection requests from clients, using the protocol and port you configure.
You define rules that determine how the load balancer routes requests to its registered targets.
Each rule has priority, one or more actions and one or more conditions.
### Rules
When the conditions of a rule are met, then its action is performed.
You must define a default rule for each listener.
Additional rules are optional.
### Target groups
They route requests to one or more registered targets using the protocol and port number you specify.
![[Pasted image 20231105224709.png]]
### HTTPS Load Balancing
To use [[HTTPS]] Listener you must deploy at least one [[SSL]]/[[TLS]] server certificate on your Load Balancer.
### Related
[[OSI Model]]
[[OSI Model|Layer 7]]
[[Elastic Load Balancer]]
[[Network Load Balancer]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/f4200e81-a7e0-4ffc-946f-f80ca08c038e/9eb52a90-c711-49c1-b2ac-17d26956392b/watch