#Databases 

### Backup types
#### On-demand
* Full backups at any time
* Zero impact on table performance
* Consistent within seconds and retained until deleted
* Operates within same [[Region]] as the source table
#### Point in time recovery (PITR)
* Protects against accidental writes or deletes
* Restore to any point in the last 35 days
* Incremental backups
* Not enabled by default
* Latest restorable: 5 minutes in the past
### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/560301d0-73d5-49db-bd06-98ac4c4d3520/9421ad81-8ebf-459c-854c-42e777bdd79a/watch