# S3 - Storage Classes

## S3 Standard - General Purpose
- High availability 
- For frequently accessed data
- Low latency and high throughput
- Use case: Big Data Analytics, mobile and gaming applications,...

## S3 Storage classes - Infrequent Access
- For data that is less frequently accessed, but requires rapid access when needed
- Lower cost than S3 standard

- Amazon S3 Standard - Infrequent Access (Use Case: Disaster Recovery, Backups)
- Amazon S3 One Zone - Infrequent Access (Use Case: Storing Secondary backup copies of on-premise data or data you can recreate)

## S3 Glacier Storage Classes
- Low cost 
- Amazon S3 Glacier Instant Retrieval 
	- Millisecond retrieval, great for data accessed once a quarter
	- Minimum storage duration of 30 days
- Amazon S3 Glacier Flexible Retrieval 
	- Expedited: 1-5 minutes, Standard: 3 to 5 hours, Bulk: 5 to 12 hours, free
	- Minimum storage duration of 90 days
- Amazon S3 Glacier Deep Archive - for long term storage
	- Standard: 12 hours, Bulk: 48 hours
	- Minimum storage duration of 180 days

## S3 Intelligent-Tiering 
- Small monthly cost for monitoring and auto-tiering free
- Moves objs automatically between Access Tiers based on usage
- No retrieval charges in S3 Intelligent Tiering 

