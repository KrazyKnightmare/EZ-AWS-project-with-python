# EZ-AWS-project-with-python
Simple AWS project using Python

Simple AWS project using Python and boto3. The script provisions a VPC, EC2 instance, S3 bucket, and configures Security Groups. This is a basic example of how to create and manage resources on AWS using Python.

Project: Basic AWS EC2 Deployment with S3 Bucket and VPC
Objective:
Create a VPC with subnets.

Launch an EC2 instance inside the VPC.

Create an S3 bucket.

Set up a Security Group to allow HTTP (port 80) and SSH (port 22) access.

What This Script Does:
VPC Creation: Creates a VPC with a CIDR block of 10.0.0.0/16.

Subnet: Creates a subnet within the VPC (10.0.1.0/24).

Security Group: Sets up a security group to allow:

SSH (port 22) from anywhere.

HTTP (port 80) from anywhere.

EC2 Instance: Launches an EC2 instance with the Amazon Linux AMI (or any valid AMI for your region) within the created subnet and applies the security group.

S3 Bucket: Creates an S3 bucket with a unique name.

Prerequisites:
IAM Permissions: The AWS credentials used must have permissions to create EC2, VPC, S3, and security groups.

EC2 Key Pair: You need to have an EC2 key pair for SSH access (your-key-pair in the script).

Region: Ensure you're running the script in the correct region where the resources should be deployed.

How to Run:
Save this Python script to a file (e.g., aws_deployment.py).

Ensure you have valid AWS credentials configured using aws configure in the terminal.

