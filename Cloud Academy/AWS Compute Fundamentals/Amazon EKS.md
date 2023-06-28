- AWS provides a managed service allowing you to run Kubernetes without having to take care of provisioning and running kubernetes management infra
- You just need to provision and maintain **worker nodes**

## Kubernetes Control Plane
- Components that make up the control plane:
	- Number of different APIs
	- Kubelet processes
	- Kubernetes Master
- It schedules containers onto nodes
	- Not time, but which container goes into which node based on their requirements
- It also tracks the state of all kubernetes objects
- In EKS, AWS is responsible for provisioning, scaling and managing the control plane

## Worker nodes
- A node is a working machine. It runs on demand EC2 Instances
- AMI is used to create these EC2 Instances