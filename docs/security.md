# AWS EC2 Monitoring & Security Project - Security

## Security Overview

Security is a key part of this project.

The environment is designed to follow AWS security best practices while maintaining controlled access to the EC2 instance and AWS resources.

## EC2 Security

The EC2 instance is protected through AWS network security controls.

Security considerations include:

- Restricting inbound network access
- Allowing only required services
- Avoiding unnecessary open ports
- Monitoring network activity
- Keeping the operating system updated

## IAM Security

IAM will be used to provide controlled access to AWS resources.

The planned configuration uses an IAM Role attached to the EC2 instance instead of storing permanent AWS access keys on the server.

Benefits include:

- No hard-coded AWS credentials
- Temporary credentials provided through the IAM Role
- Easier credential management
- Reduced risk of credential exposure
- Support for least-privilege access

### IAM Status

Status: In Progress

The IAM Role configuration will be documented after the role is created and attached to the EC2 instance.

## Network Security

The EC2 instance operates inside an Amazon VPC.

Network access is controlled using AWS security controls such as Security Groups.

The project follows the principle of allowing only the traffic required for the environment.

## Credential Security

No AWS Access Keys or Secret Access Keys are stored in the project repository.

Sensitive credentials must never be committed to Git or uploaded to GitHub.

The project also avoids placing passwords, tokens, private keys, or other secrets inside configuration files.

## GitHub Security

The project repository is managed using Git and GitHub.

SSH authentication is used for Git operations from the EC2 instance.

The SSH private key is stored only on the EC2 instance and must never be uploaded to GitHub or shared publicly.

Only the SSH public key is registered with GitHub.

## Security Best Practices

The project follows these security principles:

1. Least privilege
2. No hard-coded credentials
3. Restricted network access
4. Secure Git authentication
5. No secrets in source control
6. Regular monitoring
7. System updates
8. Controlled AWS permissions

## Planned Security Improvements

Future improvements include:

- Creating and attaching an IAM Role
- Applying least-privilege IAM permissions
- Configuring CloudWatch monitoring
- Creating CloudWatch alarms
- Enabling centralized logging
- Using AWS Systems Manager
- Automating security checks
- Documenting Security Group rules

## Security Status

| Security Component | Status |
|---|---|
| VPC Network Isolation | Completed |
| EC2 Security Group | Configured |
| SSH GitHub Authentication | Verified |
| AWS IAM Role | In Progress |
| CloudWatch Monitoring | Pending |
| Security Documentation | In Progress |
