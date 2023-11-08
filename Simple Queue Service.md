---
aliases:
  - SQS
---
#Queues #Decoupling
[[Poll Based Messaging Queue]] that allows asynchronous processing of work. 

### Settings
#### Delivery Delay
Default: 0
Max value: 15 (minutes)
#### Message size
A single message can contain up to 256KB of text in any format.
#### Encryption
Default: [[Encryption In Transit|encrypted in transit]].
It is possible to add [[Encryption at rest]], with some effort.
#### Message retention
Default: 4 days
Allowed values: 1 - 14 days
#### Polling
Default: Short
Available (and recommended): Long
Short polling means the [[SQS Consumer]] closes the connection immediately after checking for new messages and connecting back in the next interval window.
Long polling means the [[SQS Consumer]] connects, waits a little until the new message comes in. It costs less and 
#### Queue Depth
How many messages can a queue hold. This can be a trigger for [[EC2 Auto-Scaling|Auto-Scaling]].
### Queue types
#### Standard queue
* Best-effort ordering
* Could contain duplicate messages
* Nearly unlimited transactions per second
#### FIFO queue
* Guaranteed ordering from oldest to youngest
* No duplication
* 300 transactions per second 
* With batching it could potentially increase the speed to 3000 tr/s.
#### FIFO High Throughput
* Up to 9000 transactions per second without batching.
* Up to 90000 transactions per second with batching.
![[Pasted image 20231106210446.png]]
### Related
[[Dead-Letter Queue]]
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/b3c25c23-eaac-4635-90a0-5cc5e21d24f7/watch