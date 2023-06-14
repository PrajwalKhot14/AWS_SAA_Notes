# Route 53 Routing Policies
- How route 53 responds to DNS queries 
- Supports following routing policies:
	- Simple
	- Weighted
	- Failover
	- Latency based
	- Geolocation
	- Multi-Value Answer
	- Geoproximity

## Routing Policy - Simple
- Typically route traffic to a single resource
- Can specify multiple values in the same record
- If multiple values are specified then a random one is chosen by the client
- No health checks
- ![Simple](Images/simple.png)

## Routing Policy - Weighted
- Control the % of the requests that go to each specific resources 
- Weight need not sum up to 100
- Can add health checks 

## Routing Policy - Latency-based
- Redirect to the resource that has the least latency 
- Between user and AWS regions 
- Can add health checks