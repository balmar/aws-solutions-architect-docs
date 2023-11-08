### SOA Record
It stores information about:
* The name of the server that supplied the data for the zone
* The administrator of the zone
* The current version of the data file
* The default number of seconds for the time-to-live file on resource records
### NS Record
Namespace record.
It is used by the top-level domain servers to direct traffic to the content [[DNS Server]] that contains the authoritative [[DNS Record]]
### A Record
Address Record.
The A record is used by a computer to translate friendly name into [[IP Address]]
### TTL Record
Time-to-live Record.
It states for how long the [[DNS Record]] should be kept until updating.
### CNAME Record
Canonical name.
Used to resolve one domain name to another.
Can be used to consolidate different ways to access website.
They cannot be used for naked domain names (like http://google.com)
### Alias Record
They map resource record sets to load balancers, [[CloudFront]] distributions or [[S3 Bucket]].
Aliases work like a CNAME Record, where you can map one DNS name to another.
You can use it for naked domain names.