---
aliases:
  - MQ
---
#Computing #Queues 
A message broker service that helps migrate existing apps to [[AWS]].
### Main features
* Leverages many programming languages, [[Operating System|OS]], and messaging protocols
* Currently supports [[Apache ActiveMQ]] and [[RabbitMQ]] engine types,
* You can easily use existing apps without maintaining [[On-premise]] infrastructure.
### [[Amazon MQ]] vs [[Simple Notification Service|SNS]] with [[Simple Queue Service|SQS]]
* Both offers topics and queues
* Both one-to-one and one-to-many message designs
* Choose [[Amazon MQ]] for transferring apps with messaging systems implemented,
* For new apps look at [[Simple Notification Service|SNS]] with [[Simple Queue Service|SQS]].
* [[Amazon MQ]] needs private network like [[Virtual Private Network|VPN]], [[Virtual Private Cloud|VPC]], [[Direct Connect]]
* [[Simple Notification Service|SNS]] and [[Simple Queue Service|SQS]] are public by default
### [[Amazon MQ]] Brokers
It offers [[High Availability]] architectures, which depend on a broker engine type:
* For [[Apache ActiveMQ]] with active/standby deployments, one instance will remain available at all times.
* For [[RabbitMQ]] there are three broker nodes across multiple [[Availability Zone|AZs]] sitting behind a [[Network Load Balancer]].
 

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/27b98fbc-1b90-4130-b02e-2c370e250c19/wa