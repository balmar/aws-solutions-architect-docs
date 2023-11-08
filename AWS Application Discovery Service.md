#Migration 
Helps plan migrations to AWS via a collection of usage and configuration data from on-premises servers.
### Types
#### Agentless
* Agentless Collector is deployed in VMware vCenter from a OVA file
* It identifies hosts and VMs in VCenter and collects tons of metrics, such as:
	* IP and MAC address,
	* resource allocations,
	* hostnames
	* utilization.
#### Agent Based
* AWS Application Discovery Agent is deployed on all VMs and physical servers,
* It can be deployed on Windows and Linux OS,
* It collects all the metrics that the Agentless version, and also
	* static config data,
	* performance info,
	* network connections,
	* OS processes.

### Related
[[AWS Application Migration Service]]

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/1c7cb260-b6d6-4daf-9a0e-1ce05c4d7426/52a19795-1e06-4af9-851d-a345d43799df/watch