#Network 
Legacy Load Balancer operating on [[OSI Model|Layer 7]].

### Main features
* `X-Forwarded-For` header to see the original user's [[IP Address]]
* If your application stops responding, the [[Classic Load Balancer]] will respond with HTTP 504 code - it may be the web server or database server not working properly. 
* Sticky sessions allows you to bind a user's session to a specific [[Elastic Compute Cloud|EC2 Instance]]. It is important if your application is keeping its data on [[Elastic Compute Cloud|EC2]].
> [!TIP] Issues with Sticky Sessions
> If the underlying [[Elastic Compute Cloud|EC2 Instance]] goes down, users will keep getting rejected on their requests. To fix that, disable Sticky Sessions.
### Related
[[Elastic Load Balancer]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/f4200e81-a7e0-4ffc-946f-f80ca08c038e/74b5f1c5-b2fc-4a8a-8ed8-2fff99977474/wat