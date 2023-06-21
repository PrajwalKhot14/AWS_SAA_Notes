# Amazon FSx
## Amazon FSx for Windows (File Server)
- FSx for Windows is a fully managed Windows file system share drive
- Supports SMB protocol and WIndows NTFS
- Can be mounted on Linux EC2 instances
- Supports Microsoft's Distributed File System Namespaces
- Scale up to 10GB/s, millions of IOPS, 100s PB of Data
- Storage Options:
	- SSD
	- HDD

## Amazon FSx for Lustre
- Lustre is a type of parallel distributed file system, for large-scale computing 
- The name Lustre is derived from "Linux" and "cluster"
- ML and High Performance Computing 
- Video Processing, Financial Modeling, Electronic Design Automation
- Scales up to 100s GB/s, millions of IOPS, sub-ms latencies
- Storage Options:
	- SSD
	- HDD
- **Seamless integration with S3**
	- Can read S3 as a file system(through FSx)
	- Can write the output of the computations back to S3 (through FSx)

## FSx File System Deployment Options
- Scratch File System
	- Temp storage
	- Data is not replicated
	- High Burst
	- Usage: Short-term processing, optimize costs
- Persistent File System
	- Long term storage
	- Data is replicated within same AZ
	- Replace failed files within minutes
	- Usage: Long-term processing, sensitive data

## Amazon FSx for NetApp ONTAP
- File System compatible with NFS, SMB, iSCSI protocol
- Move workloads running on ONTAP or NAS to AWS
- Works with:
	- Linux,
	- Windows
	- MaxOS
	- VMware Cloud on AWS
	- Amazon Workspaces & AppStream 2.0
	- AmazonEC2, ECS and EKS
- Storage shrinks or grows automatically
- Snapshots, replications, low-cost, compression and data de-duplication 
- Point-in-time instantaneous cloning(helpful for testing new workloads)

## Amazon FSx for OpenZFS
- File System compatible with NFS
- Move workloads running on ZFS to AWS
- Works with:
	- Linux,
	- Windows
	- MaxOS
	- VMware Cloud on AWS
	- Amazon Workspaces & AppStream 2.0
	- AmazonEC2, ECS and EKS
- Up to 1 million IOPS with < 0.5ms latency
- Snapshots, compression and low-cost
- Point-in-time instantaneous cloning(helpful for testing new workloads)
