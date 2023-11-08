#Network 
[[VPC Endpoints]] are virtual devices, which enable you to privately connect your [[Virtual Private Cloud|VPC]] to supported [[AWS]] Services.

> [!INFO] Instances in your [[Virtual Private Cloud|VPC]] do not require public [[IP Address]] to communicate with resources in the service.

> [!TIP] Use case
> When you want to connect [[AWS]] services without leaving the [[AWS]] internal network.
> 
### Main features
* Horizontally [[Scaling|Scaled]]
* Redundant,
* [[High Availability|Highly Available]]
* They do not impose availability risks or bandwidth constraints
### Types of [[VPC Endpoints]]
#### Interface Endpoints
[[Elastic Network Interface]] with a private [[IP Address]].
It serves as an entry point for traffic headed to supported service. They support a large quantity of [[AWS]] services.
#### Gateway Endpoints
Similar to [[NAT Gateway|NAT Gateways]], a gateway endpoint is a virtual device you provision. It supports connection to [[Simple Storage Service|S3]] and [[DynamoDB]].

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/e895e0dc-ee49-4a4e-9252-6018c96def38/4814e73f-fa0a-411b