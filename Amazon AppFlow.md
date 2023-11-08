#Computing 

Fully managed integration service for exchanging data between [[SaaS]] and [[AWS]] services.
Pulls data records from third-party [[SaaS]] vendors and stores them in [[Simple Storage Service|S3]].
Bi-directional data transfers with limited combinations.
### Flow
Flows transfer between sources and destinations.
### Data Mapping
Determines how your source data is stored within your destinations.
### Filters
Criteria to control which data is transferred from a source to destination.
### Trigger
How the flow is initiated. 
Supported types:
* Run on demand
* Run on event
* Run on schedule.
### Use cases
* Transferring Salesforce records to [[Amazon Redshift]]
* Ingesting and analyzing Slack conversations in [[Simple Storage Service|S3]]
* Migrating Zendesk and other help desk support tickets to [[Snowflake]]
* Transferring aggregate data on a scheduled basis to [[Simple Storage Service|S3]]
### Related

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/593d3dac-575f-4c3b-bee1-54cee5a01eaf/01f280a7-6b3b-4266-9c32-c709c5aece4c/watch