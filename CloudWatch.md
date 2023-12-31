---
aliases:
  - Amazon CloudWatch
---
#Monitoring 
Monitoring and observability platform designed to give insight about [[AWS]] services.

> [!TIP] The go-to tool for monitoring
> Remember the basic checks that are included out of the box
### Main features
* System Metrics - out of the box metrics about [[AWS]] services,
* Application Metrics - after installing [[CloudWatch Agent]] you can gather information about your [[Elastic Compute Cloud|EC2 Instance]],
* Alarms - set up an alarm based on the gathered metrics,
### Metric Examples
#### Default
* CPU utilization
* Network [[Throughput]]
#### Custom
* [[Elastic Compute Cloud|EC2]] Memory Utilization
* [[Elastic Block Storage|EBS]] capacity
### Basic vs Detailed Monitoring
Basic monitoring is available through most of the AWS services. It checks the metrics each *5 minutes* by default.
Detailed monitoring usually requires an agent inside of a EC2 instance running the service and may incur costs. Default interval is *1 minute*.
### Related
[[CloudWatch Logs]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/f317ea6f-b97e-433f-9562-93422d5f924b/703c879f-9b58-4523-8aad-63cf12963dd1/watch 
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/cloudwatch-metrics-basic-detailed.html