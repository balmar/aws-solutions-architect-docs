---
aliases:
  - DLQ
  - Dead-Letter Queues
---
#Decoupling 
A [[Simple Queue Service|SQS]] queue for messages that cannot be processed successfully.

> [!TIP] If the exam scenario mentions issues with messages processing
> Think [[Dead-Letter Queue|Dead-Letter Queues]].
 ### Main features
* It is a regular [[Simple Queue Service|SQS]] queue under the hood,
* Works with [[Simple Queue Service|SQS]] and [[Simple Notification Service|SNS]].
* Useful for debugging and troubleshooting
* Redrive capability can move the message back into the source queue.
### Benefits
* You can configure alarms based on message counts
* Quickly identify which logs to investigate for exceptions
* Analyze the original [[Simple Queue Service|SQS]] messages for errors,
* Troubleshoot consumer permissions

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/197141b9-bded-4da3-8c91-12d09424c3d3/watch