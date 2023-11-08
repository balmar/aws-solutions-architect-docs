#S3 #Storage 

### Standard tiers
#### Standard
* High availability (99.99%) and durability (99.99999999%)
* Designed for frequent access
* Suitable for most cases
#### Standard-Infrequent Access (S3 Standard-IA)
* Rapid Access
* You need to pay to access the data
* Great for long-term storage, backups and a data-store
* High availability (99.9%) and durability (99.999999999%)
#### S3 One Zone-Infrequent Access (S3 One Zone-IA)
* Simmilar to *Standard-Infrequent Access*, but is stored in only one [[Availability Zone|AZ]],
* Costs 20% less than *S3 Standard-IA*
* Great for long-lived, infrequently accessed, non-critical data,
* Availability (99.5%), durability (99.999999999%)

#### S3 Intelligent Tiering (S3 IT)
* Moves objects into a specific Tiers based on AI,
* Optimizes costs, but at a cost of `$0.0025 / 1000 objects`.

### Glacier tiers
* You pay for each time you access data,
* Used only for archiving your data
* Cheap storage
* Optimized for very rarely used data

#### Glacier Instant Retrieval
* Long-term data archiving with instant retrieval time
#### Glacier Flexible Retrieval
* A storage class for data that does not require immediate access,
* Good for backups or disaster recovery use cases
* Retrieved within minutes up to 12 hours
#### Glacier Deep Archive
* Cheapest storage
* Designed for retaining data for 7-10 years,
* Standard retrieval time is 12h and bulk is 48h

### Comparison
-|S3 Standard|S3 IT|S3 Standard-IA|S3 One-Zone-IA|S3 Glacier Instant Retrieval|S3 Glacier Flexible Retrieval|S3 Glacier Deep Archive
--|--|--|--|--|--|--|--
Durability|11 9's|11 9's|11 9's|11 9's|11 9's|11 9's|11 9's|11 9's
Availability|99.99%|99.9%|99.9%|99.5%|99.9%|99.99%|99.99%
Availability SLA|99.9%|99%|99%|99%|99.9%|99.9%|99.9%
Availability Zones|>=3|>=3|>=3|1|>=3|>=3|>=3

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7202718b-2595-4fb5-9c0f-62eedc9c7820/ce3f4ad4-ac26-4f83-8c47-2cc43c256932/watc