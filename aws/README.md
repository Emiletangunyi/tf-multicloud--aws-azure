# Multi-Cloud Architecture with AWS and Azure

## Overview
This project demonstrates a multi-cloud architecture using AWS and Azure deployed with Terraform.

- AWS hosts the web server (application layer)
- Azure hosts the MySQL database (data layer)

This setup simulates a real-world distributed architecture across cloud providers.

---

## Architecture

- AWS:
  - VPC
  - Public Subnet
  - EC2 Web Server
  - Security Group

- Azure:
  - Resource Group
  - Virtual Network (VNet)
  - Subnet (delegated)
  - MySQL Flexible Server
  - Private DNS

---

## Technologies Used

- Terraform
- AWS (EC2, VPC)
- Azure (VNet, MySQL Flexible Server)
- Linux (Apache Web Server)

---

## Deployment Steps

### AWS
- Created VPC and subnet
- Deployed EC2 instance
- Installed Apache web server

### Azure
- Created Resource Group and VNet
- Configured subnet delegation
- Deployed MySQL Flexible Server

---

## Key Concepts Demonstrated

- Multi-cloud architecture design
- Infrastructure as Code (Terraform)
- Networking across cloud providers
- Secure database deployment
- Resource lifecycle management

---

## Notes

- Azure MySQL deployment required region selection based on subscription availability
- Terraform state files were excluded using `.gitignore`
- Resources were destroyed after testing to avoid unnecessary costs

---

## Future Improvements

- Connect AWS EC2 to Azure MySQL database
- Add CI/CD pipeline (GitHub Actions)
- Implement private connectivity (VPN / peering)

---

## Author

Emile Tangunyi 