# Network Load Balancer

- Network load balancers allow to:
	- Forward TCP and UDP traffic to your instance
	- Handle millions of requests per second
	- Less latency ~100 ms, ALB is ~400 ms
- NLB has one static IP per AZ, and supports assigning elastic IP
- NLB are used for extreme performance, TCP or UDP traffic
- Health checks support the TCP, HTTP and HTTPS protocols