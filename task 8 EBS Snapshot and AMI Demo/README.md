# TASK-8 : Exploring EC2, EBS Snapshots & AMIs on AWS

This project demonstrates how to preserve and reuse EC2 instance data and configurations using EBS Snapshots and Amazon Machine Images (AMIs).

## Objective

To understand:
- How to take and restore EBS Snapshots
- How to create and launch AMIs
- The difference between storage-level (snapshot) and system-level (AMI) backups
- Data portability across different EC2 instances

## Steps Performed

### 1: Launch a Base EC2 Instance
![alt text](image.png)
![alt text](image-1.png)

### 2: Connect and Add Data
![alt text](image-2.png)

### 3: Create a Snapshot of the EBS Volume
![alt text](image-3.png)

### 4: Create a New EBS Volume from Snapshot
![alt text](image-4.png)
![alt text](image-5.png)

### 5: Create an AMI from the Instance
![alt text](image-6.png)

### 6: Launch a New EC2 Instance (RHEL)
![alt text](image-7.png)

### 7: Attach the Volume (from Snapshot)
![alt text](image-8.png)
![alt text](image-9.png)

### 8: Access Snapshot Data via Terminal
- Expected output: Hello from task8-instance-1!
![alt text](image-10.png)

### Testing AMI Portability
### 9: Launch a New EC2 Instance from AMI
![alt text](image-11.png)

### 10: Verify AMI-Based Instance
![alt text](image-12.png)