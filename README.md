# Multi-Environment AWS Infrastructure Provisioning using Terraform

## Project Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to automate the provisioning and management of AWS resources across multiple environments.

The infrastructure is designed to support Development (Dev), Staging (Stg), and Production (Prd) environments using reusable Terraform configurations and variables.

---

## Objective

The objective of this project is to automate AWS infrastructure deployment using Terraform and implement Infrastructure as Code (IaC) best practices.

### Goals

- Provision AWS resources using Terraform
- Create reusable and scalable infrastructure
- Manage multiple environments (Dev, Staging, Production)
- Automate infrastructure deployment
- Reduce manual configuration efforts
- Gain hands-on experience with Terraform and AWS services

---

## Architecture

```text
Terraform
    │
    ▼
AWS Cloud
    │
    ├── Development Environment
    │      ├── EC2 Instances
    │      ├── S3 Bucket
    │      └── DynamoDB Table
    │
    ├── Staging Environment
    │      ├── EC2 Instances
    │      ├── S3 Bucket
    │      └── DynamoDB Table
    │
    └── Production Environment
           ├── EC2 Instances
           ├── S3 Bucket
           └── DynamoDB Table
```

---

## AWS Services Used

- Amazon EC2
- Amazon S3
- Amazon DynamoDB
- Security Groups
- Key Pairs
- IAM
- Terraform

---

## Features

- Infrastructure as Code (IaC)
- Multi-Environment Deployment
- Automated AWS Resource Provisioning
- Reusable Terraform Configuration
- Terraform Variables and Outputs
- Data Sources for Dynamic Resource Selection
- Scalable Infrastructure Design

---

## Resources Created

### Compute

- EC2 Instances
- Key Pair
- Security Groups

### Storage

- Amazon S3 Bucket

### Database

- Amazon DynamoDB Table

---

## Project Structure

```text
terraform-aws-infrastructure/
│
├── main.tf
├── ec2.tf
├── s3.tf
├── db.tf
├── variables.tf
├── outputs.tf
│
├── screenshots/
│   ├── terraform-plan.png
│   ├── terraform-apply.png
│   ├── ec2-instances.png
│   ├── s3-bucket.png
│   └── dynamodb-table.png
│
└── README.md
```

---

## Prerequisites

Before running the project, ensure you have:

- AWS Account
- AWS CLI Configured
- Terraform Installed
- IAM User with Required Permissions

Verify installation:

```bash
terraform -version
aws --version
```

---

## Terraform Workflow

### Initialize Terraform

```bash
terraform init
```

### Validate Configuration

```bash
terraform validate
```

### Generate Execution Plan

```bash
terraform plan
```

### Create Infrastructure

```bash
terraform apply
```

### Destroy Infrastructure

```bash
terraform destroy
```

---

## Variables

The project uses Terraform variables to create reusable infrastructure across multiple environments.

Example:

```hcl
environment = "dev"
instance_type = "t2.micro"
```

Supported environments:

- dev
- stg
- prd

---

## Outputs

After deployment, Terraform provides outputs such as:

- Instance IDs
- Public IP Addresses
- S3 Bucket Names
- DynamoDB Table Names

---


## Learning Outcomes

Through this project, I gained hands-on experience in:

- Terraform Fundamentals
- Infrastructure as Code (IaC)
- AWS Resource Provisioning
- Terraform Variables and Outputs
- Multi-Environment Infrastructure Management
- State Management
- AWS Compute, Storage, and Database Services

---

## Note

This project was successfully deployed and tested using Amazon S3 Static Website Hosting and GitHub Actions. The AWS resources were later removed to avoid ongoing cloud costs.

---

## Author

Sneha Alhat

Aspiring Cloud & DevOps Engineer

Skills:
AWS | Terraform | Git | GitHub | Linux | CI/CD | Cloud Computing
