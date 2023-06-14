- Highly available, scalable, fully managed and Authoritative DNS
	- Authoritative = the customer can update the DNS records
- It is also a domain Registrar
- Ability to check health of your resources
- 100 % Availability
- 53 is a reference to the traditional DNS port

## Route 53 - Records 
- Each record contains
	- Domain/subdomain Name - eg: example.com
	- Record Type - eg: A or AAAA
	- value - eg: 12.34.56.78
	- Routing Policy: how route 53 responds to the query
	- TTL - amount of time the record is cached at DNS resolvers
- Route 53 supports following DNS record types: 
	- A / AAAA / CNAME / NS (Must Know)
		- A - maps a hostname to IPv4
		- AAAA - maps a host to IPv6
		- CNAME - maps a hostname to another hostname
			- Target is a domain name which can be A or AAAA record
			- Can't create a CNAME record for the top node of a DNS namespace
			- Example: you can't create for example.com but you can create for www.example.com
		- NS - Name Servers for the Hosted Zone

## Hosted Zones
- A container for records that define how to route traffic to a domain and its subdomains
- **Public Hosted Zones** - contains records that specify how to route traffic on the internet
- **Private Hosted Zones** - contains records that specify how to route traffic within one or more VPCs