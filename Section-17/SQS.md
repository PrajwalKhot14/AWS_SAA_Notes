## Amazon SQS - Standard Queue
- Used to decouple applications
- Attributes:
	- Unlimited throughput, unlimited number of messages in queue
	- Default retention of messages: 4days
	- Max: 14 days
	- Low latency (<10 ms on publish and receive)
	- Limitation of 256 KB per message
- Can have duplicate messages
- Can have out of order messages

### SQS - Producing Messages
- Produced to SQS using SDK (SendMessage API)
- Message is persisted in SQS until consumer deletes it
- default 4 days, max 4 days retention 

### SQS - Consuming Messages
- Receive up to 10 messages at a time
- Delete the message using DeleteMessage API

There can be multiple producers and consumers