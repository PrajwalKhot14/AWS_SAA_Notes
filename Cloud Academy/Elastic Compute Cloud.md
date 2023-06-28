# EC2 Instances
## Amazon Machine Images (AMI)
- These are templates of preconfigured EC2 instances
- There is a marketplace for this
- We can create our own and save it as a template

## Instance Types
- Micro Instances: t1, t2, t3.micro
- General Instances
- Compute Optimized: have higher ratio of vCPUs to memory. For CPU-bound scale out applications. Ex: High perfomance, batch processing..
- FPGA Instances: 
- GPU Instances: HPC, 3-D graphics, rendering...
- Memory Optimized: High RAM
- Storage Optimized: High IO

## Instance Purchase Options
- On-Demand Instances: 
	- Can be launched any time
	- Flat rates
	- For short term
	- For dev and test env
- Reserved Instances
	- For a period of time
	- 1 or 3 years
- Scheduled Instances:
	- reserve on a recurring schedule
	- daily, weekly, monthly
	- You will be charged even if not used
- Spot Instances:
	- bid for EC2
	- Not guaranteed 
- On-Demand Capacity Reservations