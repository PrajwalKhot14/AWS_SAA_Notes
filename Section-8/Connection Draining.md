# Connection Draining

- Time to complete "in-flight requests" while the instance is de-registering or unhealthy
- Stops sending new requests to the EC2 instance which is de-registering
- Between 1 to 3600 seconds 
- Can be disabled 

Connection Draining - CLB
Reregistration Delay - ALB and NLB