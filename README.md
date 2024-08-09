AWS CloudFormation Template

*Description:*
This AWS CloudFormation template provisions the following resources in your AWS environment:


VPC with two subnets (public and private)

Internet Gateway attached to the VPC

Route tables for public and private subnets

Security group allowing SSH and HTTP access

EC2 instance in the public subnet


*Prerequisites:*

An AWS account with necessary permissions.
An existing SSH key pair in your AWS account (referenced as Skillsync-Key in the template).


*Usage:*

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
