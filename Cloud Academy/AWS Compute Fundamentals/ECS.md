# ECS
- Run docker enabled applications 
- ECS clusters are region specific

## AWS Fargate
- Engine used to enable ECS to run containers

## Launching an ECS Cluster
- Fargate launch:
	- Required you to specify the CPU and memory required, 
	- define networking and IAM policies
- EC2 launch:
	- You are responsible for patching and scaling your instances
	- Instance type
	- How many containers in each cluster

## Monitoring Containers
- Done using Amazon CloudWatch
- Can create alarms based on metrics

