---
aliases:
  - API Gateways
---
Fully managed service for creating, publishing, maintaining, monitoring and securing your [[Application Programmable Interface|API]].

Create a "front door" entrance for your [[Application Programmable Interface|API]].
Integrates well with [[Lambda]], [[HTTP]] endpoints etc.
> [!TIP] Exam scenario for creating / managing [[API]]?
> Think [[API Gateway]]
### Main features
#### Security
Allows to easily protect your endpoints by attaching a [[Web Application Firewall]]
#### Stops abuse
Easy to deploy [[Distributed Denial Of Service|DDOS]] protection
#### Simplicity
Build powerful [[Application Programmable Interface|API]]s in a simple manner

### [[Application Programmable Interface|API]] Options
#### [[REST]] API
API keys, per-client throttles, validation of requests, [[Web Application Firewall|WAF]] integration.
#### [[HTTP]] API
A simpler option, cheaper and minimal
#### [[WebSocket]] API
A collection of [[WebSocket]] routes integrated with [[Lambda|Lambdas]], [[HTTP]] Endpoints and other [[AWS]] services
### Endpoint types
#### Edge-optimized
A default option. [[Application Programmable Interface|API]] requests get sent through [[CloudFront]] [[Edge Location]]. Best for global user base.
#### Regional
Perfect for clients that reside in the same, specific [[Region]].
Ability to also leverage with [[CloudFront]], if required.
#### Private
Only accessible via [[Virtual Private Cloud|VPCs]] using interface [[Virtual Private Cloud|VPC]] endpoints.

### Securing APIs
* You can add [[User Authentication]] at [[Application Programmable Interface|API]] level
* For [[Authentication]] you can use [[IAM Role|IAM Roles]], [[Amazon Cognito]] or your own custom authorizer using [[Lambda|Lambdas]].
* Edge-optimized endpoints require [[ACM]] certs in `us-east1`
* Regional endpoints require [[ACM]] certs in the same [[Region]]
* You can add [[Web Application Firewall|WAF]] in front of your [[Application Programmable Interface|API]] for [[Distributed Denial Of Service|DDOS]] protection
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/9a4f919a-f32e-4ed2-9d86-195b656380ae/watch