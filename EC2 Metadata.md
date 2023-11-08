---
aliases:
  - Metadata
---
#Computing 
A information about server which is accessible only from the source machine.
To access those information you need to `curl` to `http://169.254.169.254/latest/metadata`.
There are a lot of possible metadata you can retrieve, such as:
* ami-id,
* hostname,
* instance-id
* instance-type,
* network,
* public-ipv4,
* security-groups,
* etc.

You can use [[User Data]] to access [[EC2 Metadata]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/c91a47a3-9bdd-424e-89dd-71c9c866d736/07e8512f-3e4a-4950-9650-c63658c366e1/watch