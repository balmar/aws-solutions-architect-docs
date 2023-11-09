#Network 
*AWS Global Accelerator* is a networking service that helps you improve the availability, performance, and security of your public applications. 

*Global Accelerator* provides two global static public IPs that act as a fixed entry point to your application endpoints, such as [[Application Load Balancer]], [[Network Load Balancer]], [[Elastic Compute Cloud|EC2 Instances]], and [[Elastic IP Address]].
### Important Capabilities
#### Automation
Use predefined or custom playbooks to enable resource management.
#### Run Command
Remotely execute commands on managed compute without [[SSH]] or [[RDP]].
#### Patch Manager
Automates patching managed instances (OS patches and applications)
#### Parameter Store
Securely store your secrets and application configuration information.
#### Maintenance Windows
Define a schedule for performing actions on your managed instances.
#### Session Manager
Securely connect to your managed compute without needing [[SSH]] access, so you don't have to expose any ports. Every action can be logged into [[CloudWatch]] and [[AWS CloudTrail|CloudTrail]].

### Use cases
* Global traffic manager
* API acceleration
* Global static IP
* Low-latency gaming and media workloads
### Source
https://aws.amazon.com/g