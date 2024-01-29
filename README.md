# Highly Available AWS Cloud-Based Web Application directory

## Introduction
AWS-powered web application project, designed for high availability and resilience. This is AWS based.

## Architecture
The application is architected for high availability across multiple Availability Zones (AZs) in the US East (N. Virginia `us-east-1`) and US East (Ohio `us-east-2`) regions, ensuring reliable and consistent access.

### AWS Services and Features
- **Virtual Private Cloud (VPC)**: Configured with 6 subnets spanning 2 different AZs for redundancy and fault tolerance.
- **Subnets**:
  - Public Subnet: Provides access to the Internet for the EC2 instances.
  - Private Subnet (EC2): Hosts the web application instances, isolated for security.
  - Private Subnet (Database): Reserved for future database implementations, currently not in use due to DynamoDB's managed service.
- **DynamoDB**: Serves as the scalable and managed NoSQL database solution.
- **Amazon S3**: Utilized for storing and retrieving application images, integrated with DynamoDB.
- **Security Groups**: Configures firewall rules to control traffic to EC2 instances.
- **Target Groups**: Directs traffic to appropriate EC2 instances via the Application Load Balancer.
- **Application Load Balancer (ALB)**: Distributes incoming application traffic across multiple targets, such as EC2 instances, in multiple Availability Zones.
- **Auto Scaling Groups**: Automatically adjusts the number of EC2 instances in response to traffic demands.

## Additional AWS Components
The project incorporates various other AWS services to enhance functionality, including IAM Roles for security best practices and launch templates for EC2 instances provisioning.

## Repository Contents
Within this repository, you will find:
- **CloudFormation Templates**: The `CloudFormation` directory contains all the YAML templates used to define the AWS resources.
- **AWS Console & Website Screenshots**: The `AWS Console and Website running-Images` directory provides a visual insight into the AWS Console's behavior and the web application's responses.

## Architecture
a Highly available web app that use different AWS services to run,like:
- VPC with 6 subnets within 2 different AZ (us-east-1 and us-east-2) for high availability
- Each AZ contains 1 public Subnet, 1 private subnet for the EC2 app, and 1 private subnet for the Database (not used on this case due to the use of Dynamo DB)
- A Dynamo DB table as a database for scalability and easy management.
- S3 for storing the app images retrieval to the Database DynamoDB
- Security Groups
- Target Groups poiting by the Application Load Balancer
- Application Load Balancerto balance the workload
- AutoScaling Groups

And other services like IAM Roles, launch templates and more, you can find my CloudFormation YAML templates code on this REPOSITORY

On the folder AWS Console and Website running-Images you will find images of the AWS Console behavior and the web site responses

[![LinkedIn](https://www.linkedin.com/in/giogalindo470/)](Tu-URL-de-LinkedIn)
https://www.linkedin.com/in/giogalindo470/

