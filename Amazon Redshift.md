---
aliases:
  - Redshift
---
#Databases #BigData 
Fully managed, petabyte-scale data warehouse service in the cloud.
A very large [[Relational Database]] traditionally used in [[Big Data]] apps.
### Size
[[Amazon Redshift|Redshift]] is big - it can hold up to 16PB of data. You don't have to split up your large databases.
### Relational
It is a [[Relational Database]], so you can use your standard [[SQL]] and [[BI]] tools to interact with it.
### Based on [[PostgreSQL]]
This is based on the [[PostgreSQL]] database engine type; however it is *NOT* meant for [[Online Transaction Processing|OLTP]] loads.
### Usage
It is meant to replace standard [[Relational Database Service|RDS]] databases.
### High Performance
Offers up to 10x the performance of other data warehouses offered in the cloud.
### Columnar
Storage of data is column-based instead of row-based. Allows for efficient parallel queries.
### High Availability
[[Amazon Redshift|Redshift]] supports [[Multi-AZ RDS]]. It only spans two [[Availability Zone|AZs]] for now.
You cannot shift between Single-[[Availability Zone|AZ]] and Multi-[[Availability Zone|AZ]]
### Snapshots
Incremental [[Snapshot|Snapshots]] are incremental and point-in-time. They can be automated or manual. Stored in [[Simple Storage Service|S3]]
### Redshift Spectrum
Efficiently query and retrieve data from [[Simple Storage Service|S3]] without having to load the data into [[Amazon Redshift|Redshift]] tables. It is extremely fast against large datasets.
### Enhanced [[Virtual Private Cloud|VPC]] Routing
All *COPY* and *UNLOAD* traffic between your cluster and your data repositories is forced through your [[Virtual Private Cloud|VPC]]. It enables you to use [[VPC Endpoints]], [[VPC Flow Logs]] etc.

> [!TIP] Always favor large batches!
> If you have a scenario about optimizing [[Amazon Redshift|Redshift]], you should favor big data batches
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/7bcd3ba2-1d13-4c67-92c4-2e979998a4fd/6150960b-1f5f-49d6-baa8-5e4b0ab43f6c/wa