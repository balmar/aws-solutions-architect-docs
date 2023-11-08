---
aliases:
  - AWS Health
tags:
  - Compliance
---
* See resource performance and availability of AWS services / accounts.
* You can see how the health events affect you and your services.
* It is meant to be quick and relevant,
* You can view upcoming maintenance tasks,
* It almost immediately notifies you on any alerts
### Keywords
#### AWS Health event
Notification sent on behalf of AWS services.
#### Account specific event
Event that impacts certain account.
#### Public event
Events on public services
#### AWS Health Dashboard
Dashboard showing account and public events
#### Event
It will contain properties such as:
* type code,
* type category,
* status,
* affected entities.

#### Event examples
* AWS_EC2_SYSTEM_REBOOT_MAINTENANCE_SCHEDULED
	* The machine that the [[Elastic Compute Cloud]] operates on will reboot.
* AWS_EC2_OPERATIONAL_ISSUE
	* Some of the AWS services are encountering delays or downtimes.
* AWS_BILLING_SUSPENSION_NOTICE
	* Sent when there are outstanding charges and the account is at risk of suspension or closure.


>  Pro tip: You can automate actions based on incoming events using Amazon EventBridge


