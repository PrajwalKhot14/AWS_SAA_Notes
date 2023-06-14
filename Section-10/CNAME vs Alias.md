# CNAME vs Alias
AWS Resources expose AWS hostname:
	ib1-1234.us-east-2.elb.amazonaws.com and you want myapp.mydomain.com
- CNAME: 
	- Points a hostname to any other hostname 
		- app.mydomain.com => blahblah.anything.com
	- Only for non root domain (aka.something.mydomain.com)
- Alias:
	- Points a hostname to an AWS Resource
	- Works for ROOT DOMAIN and NON ROOT DOMAIN
	- Free of charge

## Route 53 - Alias Records
- Unlike CNAME, it can be used for the top node of a DNS namespace. Eg: example.com
- Always of type A/AAAA for AWS resources
- Can't set TTL