---
aliases:
  - S3 Event Notification
---
You can use the Amazon S3 Event Notifications feature to receive notifications when certain events happen in your S3 bucket. To enable notifications, add a notification configuration that identifies the events that you want Amazon S3 to publish. Make sure that it also identifies the destinations where you want Amazon S3 to send the notifications. You store this configuration in the _notification_ subresource that's associated with a bucket.
### Possible event triggers
[[S3 Event Notifications]] could be trigged by:
- New object created events
- Object removal events
- Restore object events
- Reduced Redundancy Storage (RRS) object lost events
- Replication events
- S3 Lifecycle expiration events
- S3 Lifecycle transition events
- S3 Intelligent-Tiering automatic archival events
- Object tagging events
- Object ACL PUT events
### Viable notification targets
* [[Simple Notification Service|SNS]]
* [[Simple Queue Service|SQS]]
* [[Lambda]]
* [[Amazon EventBridge]]
### Source
https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventNotificati