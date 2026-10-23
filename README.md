# EWB-AWS-VPC-Peering
AWS VPC Peering project with two VPCs, private EC2 instances, route tables, security groups, bastion SSH, and connectivity testing.
# AWS VPC Peering Project

## Project Overview
This project demonstrates VPC Peering between two Amazon Web Services (AWS) Virtual Private Clouds (VPCs) to enable private communication between EC2 instances.

## Architecture

- **VPC A:** `10.10.0.0/16`
- **VPC B:** `10.20.0.0/16`
- **Bastion Host:** `10.10.1.10`
- **App-A EC2:** `10.10.2.10`
- **App-B EC2:** `10.20.1.10`
- **VPC Peering:** `ewb-a-b-peer`

## AWS Services Used
- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- SSH and ICMP Connectivity Testing

## Implementation
1. Created two VPCs with separate CIDR ranges.
2. Launched a bastion host and two application EC2 instances.
3. Created and activated a VPC peering connection.
4. Configured routes in the required route tables.
5. Configured security groups for SSH and ICMP traffic.
6. Tested connectivity between App-A and App-B in both directions.
7. Tested SSH access to private instances through the bastion host.
8. Tested ICMP failure and recovery by temporarily changing a security group rule.

## Results
- App-A to App-B connectivity: Successful.
- App-B to App-A connectivity: Successful.
- SSH through the bastion host: Successful.
- Security group failure and recovery test: Completed successfully.

## Learning Outcomes
Learned how VPC peering, routing, security groups, bastion hosts, and private EC2 connectivity work in AWS.

## Security Note
No private keys, passwords, access tokens, or other sensitive credentials should be included in this repository.

## Cleanup
AWS resources should be terminated or deleted after testing to avoid unnecessary charges.
