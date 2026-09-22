# AWS CloudFormation Demo Stack — VPC + RDS Infrastructure

## Project Overview
Provisioned a complete AWS cloud infrastructure using CloudFormation 
(Infrastructure as Code) including a VPC, private subnets, security 
groups, and an RDS MySQL database — all automated via a single stack.

## Architecture
- **VPC** (192.168.0.0/16) — Isolated network environment
- **Private Subnet 1** (192.168.1.0/24) — ap-south-1b
- **Private Subnet 2** (192.168.2.0/24) — ap-south-1c
- **Security Group** — MySQL port 3306 access control
- **RDS Subnet Group** — Multi-AZ subnet grouping
- **RDS MySQL 8.0** (db.t3.micro) — Database instance

## AWS Services Used
- AWS CloudFormation
- Amazon VPC
- Amazon RDS (MySQL 8.0.42)
- Amazon EC2 (Security Groups, Subnets)
- Amazon S3

## What I Learned
- Writing CloudFormation templates (Infrastructure as Code)
- Designing VPC networking with private subnets
- Deploying RDS databases inside a VPC
- Managing cloud resources and cost optimization
- Deleting stacks to avoid unnecessary AWS charges

## Region
ap-south-1 (Mumbai, India)

## Steps to Deploy
1. Go to AWS CloudFormation Console
2. Create Stack → Upload template
3. Enter stack name: `demostack`
4. Click Create — all resources provision automatically