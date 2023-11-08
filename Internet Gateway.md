#Network 

An **internet gateway** is a horizontally scaled, redundant, and highly available [[VPC]] component that allows communication between your [[VPC]] and the internet. 

It supports IPv4 and IPv6 traffic. It does not cause availability risks or bandwidth constraints on your network traffic.

> [!TIP] Subnets need a route in [[Route Table]] to access the internet through the [[Internet Gateway]]

> [!TIP] Instances in your subnet must have either IPv4 or IPv6
### Source
https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html