# S3 Encryption

4 Methods to encrypt

- Server-Side Encryption (SSE)
	- SSE with Amazon S3 Managed Keys(SSE-S3) - Enabled by default
		- Encrypts S3 objects using keys handled, managed and owned by AWS
	- SSE with KMS keys stored in AWS KMS (SSE-KMS)
		- Leverage AWS Key Management Service (AWS KMS) to manage encryption keys
	- SSE with Customer-Provided Keys(SSE-C)
		- When you want to manage your own encryption keys
- Client-Side Encryption

## SSE S3
- Encrypts S3 objects using keys handled, managed and owned by AWS
- Objs are encrypted server-side
- AES-256
- Must set header "x-amz-server-side-encryption":"AES256"

## SSE KMS
- Encryption using keys handled and managed by AWS KMS
- KMS adv: User control + audit key usage using CloudTrail
- Objs are encrypted server-side
- Must set header "x-amz-server-side-encryption":"aws:kms"
- Limitation:
	- You may be impacted by the KMS limits
	- When you upload, it calls the GenerateDataKey KMS API
	- When you download, it calls the Decrypt KMS API
	- All the calls count towards the KMS quota per second

## SSE C
- SSE using keys fully managed by customer outside of AWS
- Amazon S3 does NOT store the encryption key you provide
- HTTPS must be used
- Encryption key must provided in the HTTP headers, for every HTTP request made


## Client-Side Encryption
- Use client libraries such as Amazon S3 Client-Side Encryption Library 
- Clients must encrypt data themselves before sending the data to Amazon S3
- decrypt as well