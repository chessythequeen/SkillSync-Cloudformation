# AWS CloudFormation Template 

This repository contains an AWS CloudFormation template that automates the creation of a Virtual Private Cloud (VPC), EC2 instances, and associated security groups. This template is designed to set up a basic network infrastructure on AWS, including public and private subnets, internet gateway, and route tables.

## Template Overview

The CloudFormation template (`SkillSync.yaml`) included in this repository will create the following resources:

- **VPC**: A Virtual Private Cloud with DNS support and hostnames enabled.
- **Internet Gateway**: An Internet Gateway attached to the VPC.
- **Subnets**: 
  - A public subnet in the VPC.
  - A private subnet in the VPC.
- **Route Tables**: 
  - A public route table associated with the public subnet.
  - A private route table associated with the private subnet.
- **Security Group**: A security group allowing SSH (port 22) and HTTP (port 80) access.
- **EC2 Instance**: An Amazon Linux 2 EC2 instance in the public subnet, associated with the security group.

## Prerequisites

Before deploying the CloudFormation template, ensure that the following prerequisites are met:

- An AWS account with the necessary permissions to create resources.
- A Key Pair created in your AWS account to access the EC2 instance via SSH. Specify the Key Pair name in the `Skillsync-Key property of the EC2 instance.
- AWS CLI or AWS Management Console to deploy the CloudFormation template.

## Deployment Instructions

Create a CloudFormation Stack:

Navigate to the CloudFormation service in the AWS Management Console.

Choose "Create Stack".

Select "Template is ready" and paste the contents of this template into the template body.

Specify a stack name and any necessary parameters.

Click "Next" to configure stack options.

Review the template and click "Create".

Monitor Stack Creation:

The CloudFormation stack creation process may take several minutes.
Monitor the stack status in the CloudFormation console.

