---
aliases:
  - SNS
---
#Monitoring #Decoupling 
[[Push Based Messaging Service]] available on [[AWS]].
It delivers messages to every subscribed observer.
Could be used for delivering notifications about alerts.

> [!TIP] If the scenario involves alerting
> Think [[Simple Notification Service]]
### Main features
#### Available Subscribers
* [[Kinesis Data Firehose]],
* [[Simple Queue Service|SQS]],
* [[Lambda]],
* email,
* [[HTTP]]/[[HTTPS]]
* SMS
* platform app endpoint
#### Message size
Up to 256 KB.
#### Types
[[FIFO]] queue (ordered, deduplicated)
Standard queue
#### On broken messages
[[Dead-Letter Queue|Dead-Letter Queues]] are supported
#### Encryption
Default: [[Encryption In Transit]]
Available: [[Encryption at rest]]
#### Access Policies
A [[Resource Policy]] can be added to a [[SNS Topic]]
#### Large Message Payloads
[[SNS Extended Library]] supports sending message of up to 2GB. They are stored in [[Simple Storage Service|S3]] and a consumer receives a reference to the object.
#### Message Filtering
Default: Messages are sent to all subscribers
Available: Adding [[Filter Policies]] to define which messages should be sent to which subscribers
#### Retry Policies
Only available for [[HTTP]]/[[HTTPS]] endpoints
### Related
[Fanout](https://en.wikipedia.org/wiki/Fan-out_(software))
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/0a53446e-bf7f-4599-ae9b-f244cada056b/watch