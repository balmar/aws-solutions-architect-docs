---
aliases:
  - Containers
---
Use containers to Build, Share and Run your applications.

Package Software into Standardized Units for Development, Shipment and Deployment.
### Containers vs Virtual Machines
#### Containers
*Containers* are an abstraction at the app layer that packages code and dependencies together. Multiple containers can run on the same machine and share the [[OS kernel]] with other containers, each running as isolated processes in user space. *Containers* take up less space than [[VM|VMs]] (container images are typically tens of MBs in size), can handle more applications and require fewer [[VMs]] and [[Operating System]]s.
#### Virtual Machines
Virtual machines ([[VMs]]) are an abstraction of physical hardware turning one server into many servers. The [[Hypervisor]] allows multiple [[VMs]] to run on a single machine. Each VM includes a full copy of an [[Operating System]], the application, necessary binaries and libraries – taking up tens of GBs. VMs can also be slow to boot.
### Source
https://www.docker.com/resources/what-container/