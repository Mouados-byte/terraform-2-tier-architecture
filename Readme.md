## 2-Tier-Architecture Project with Terraform and AWS

This project showcases implementing a scalable and resilient 2-tier architecture using Terraform and AWS. Leveraging the power of infrastructure as code, this setup provides a solid foundation for deploying web applications with high availability and fault tolerance.

## Workflow
![image](https://github.com/user-attachments/assets/c1bfa007-be71-41dc-8026-42de56850fae)


### Features
- **Tier 1: Web Tier**

  - EC2 instances provisioned in public subnets
  - Auto Scaling Group for handling the dynamic workload
  - Load Balancer for distributing traffic and ensuring high availability
  - Security Groups to control inbound and outbound traffic

- **Tier 2: Database Tier**

  - RDS MySQL instance in a private subnet
  - Secure network access using security groups

## Prerequisites
To use this project, you need to have the following prerequisites:

- AWS account with necessary permissions
- Terraform installed on your local machine

## Getting Started

1. Clone this repository to your local machine.
2. Navigate to the project directory.

```bash
$ cd 2-Tier-Architecture
```

3. Configure your AWS credentials by setting the environment variables or using the AWS CLI.
4. Initialize the Terraform project.
```bash
$ terraform init
```
5. Review the execution plan.
```bash
$ terraform plan
```
6. Deploy the architecture.
```bash
$ terraform apply
```

7. Confirm the deployment by typing `yes` when prompted.

## Cleanup
- To clean up and destroy the infrastructure created by this project, run the following command:

```bash
$ terraform destroy
```
