# AWS EC2 Monitoring & Security Project - Architecture

## Overview

This project demonstrates the deployment, configuration, security, monitoring, and troubleshooting of an Amazon EC2 Linux environment.

The architecture is designed to provide a secure and manageable cloud server environment using AWS networking, IAM, and CloudWatch services.

## Architecture Components

### Amazon VPC

The EC2 instance runs inside an Amazon VPC.

The VPC provides the network boundary for the infrastructure and controls communication between AWS resources and external networks.

### Amazon EC2

The project uses an Amazon EC2 Linux instance as the primary compute resource.

The server is used for:

- Linux administration
- Network connectivity testing
- AWS CLI operations
- Monitoring validation
- Troubleshooting
- Project documentation

### Internet Connectivity

The EC2 instance uses AWS networking to communicate with the Internet.

Outbound connectivity was validated using HTTPS requests and DNS resolution.

HTTPS connectivity test:

