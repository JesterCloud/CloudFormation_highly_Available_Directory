**AWS cloud based project, of a highly available web app directory using Load Balancers and Autoscaling Group it contains: **

# Highly Available AWS Cloud-Based Web Application

## Introduction
Welcome to our AWS-powered web application project, designed for high availability and resilience. This project leverages the robust AWS cloud infrastructure to deliver a seamless and scalable web service experience.

## Architecture
The application is archite

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

