# AWS EC2 Monitoring & Security Project

A hands-on AWS infrastructure project focused on deploying, securing, monitoring, troubleshooting, and documenting an Amazon EC2 environment.

## Project Overview

This project demonstrates practical cloud and Linux administration skills through an AWS EC2 environment.

The project covers:

- Amazon EC2
- AWS networking
- IAM Roles
- CloudWatch monitoring
- Linux administration
- DNS and Internet connectivity
- Security best practices
- Troubleshooting
- Technical documentation
- Git and GitHub

## Architecture

```text
                         Internet
                            |
                            | HTTPS
                            v
                    +---------------+
                    |   AWS VPC     |
                    +-------+-------+
                            |
                            v
                    +---------------+
                    |     EC2       |
                    | Linux Server  |
                    +-------+-------+
                            |
             +--------------+--------------+
             |              |              |
             v              v              v
           DNS          IAM Role      CloudWatch
        Resolution     Permissions     Monitoring
eof
## License

This project is intended for educational and portfolio purposes.
