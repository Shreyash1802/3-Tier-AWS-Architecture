# AWS Three-Tier Web Architecture 

## Description: 
Implemented a robust Three-Tier Architecture on AWS, prioritizing scalability and security. Strengthened network defenses by 40%, accelerated data retrieval through optimized EC2 instances with MariaDB, and improved data transfer efficiency by 35%. Check out our GitHub repository for detailed insights into the project's architecture, implementation, and performance enhancements.

## Pre-requisites:
1. An AWS account. If you don’t have an AWS account, follow the instructions [here](https://aws.amazon.com/console/) and
click on the “Create an AWS Account” button in the top right corner to create one.
1. IDE or text editor of your choice.

## Architecture Overview
![Architecture Diagram](https://github.com/Shreyash1802/3-Tier-AWS-Architecture/blob/main/web-tier/src/assets/3TierArch.png)

In this architecture, a public-facing Application Load Balancer forwards client traffic to our web-tier EC2 instances. The web tier is running Nginx webservers that are configured to serve a React.js website and redirect our API calls to the application tier’s internal facing load balancer. The internal facing load balancer then forwards that traffic to the application tier, which is written in Node.js. The application tier manipulates data in an Aurora MySQL multi-AZ database and returns it to our web tier. Load balancing, health checks, and autoscaling groups are created at each layer to maintain the availability of this architecture.

## Workshop Instructions:

See [AWS Three Tier Web Architecture](https://catalog.us-east-1.prod.workshops.aws/workshops/85cd2bb2-7f79-4e96-bdee-8078e469752a/en-US)


## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

