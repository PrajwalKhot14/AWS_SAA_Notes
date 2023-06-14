# Route 53 Health Checks
- 15 health checkers will check the endpoint health
	- Interval - 30 seconds
	- Supports HTTP, HTTPS, TCP
	- if > 18% health checkers report healthy then healthy else unhealthy
- 2xx or 3xx status code pass
- if text based then checks first 5120 bytes for pass/fail
- Configure your router/firewall to allow incoming requests from Route 53 Health Checkers
