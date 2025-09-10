<p align="center">
  <img src="https://www.vectorlogo.zone/logos/terraformio/terraformio-icon.svg" alt="Terraform Logo" width="110">
</p>

<h1 align="center">Terraform</h1>
<p align="center">Learning Journal & Practice Repository</p>

<p align="center">
  <img alt="Tool" src="https://img.shields.io/badge/IaC-Terraform-623CE4?logo=terraform&logoColor=white">
  <img alt="Cloud" src="https://img.shields.io/badge/Cloud-Any-blue">
  <img alt="Status" src="https://img.shields.io/badge/Status-In%20Progress-success">
</p>

---

## Table of Contents
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Quick Start](#quick-start)
- [Classes & Practice](#classes--practice)
- [Handy Commands](#handy-commands)
- [Project Structure (Suggested)](#project-structure-suggested)
- [Docs & Resources](#docs--resources)
- [Notes](#notes)
- [License](#license)

---

## Overview
This repository documents my **Terraform learning journey**.  
I’ll store study notes, example configurations, and lab exercises for different providers (AWS, GCP, Azure, Linode, etc.).

---

## Prerequisites
- Terraform (latest stable version) → [Install Guide](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)  
- A cloud provider account (AWS, GCP, Azure, Linode, etc.)  
- Configured credentials (via CLI or environment variables)

---

## Quick Start
```bash
# 1) Verify installation
terraform version

# 2) Initialize project (download providers, set up backend)
terraform init

# 3) Validate syntax
terraform validate

# 4) See execution plan
terraform plan

# 5) Apply infrastructure
terraform apply

# 6) Destroy infrastructure
terraform destroy
Classes & Practice
 Day 1 — Install Terraform, CLI basics, providers

 Day 2 — Variables, outputs, terraform.tfvars

 Day 3 — State files, remote backends

 Day 4 — Provisioners, modules

 Day 5 — Workspaces & environments

 Day 6 — Real cloud project (e.g., AWS VPC, EC2, S3)

Handy Commands
bash
Copy code
# Format code (fix indentation)
terraform fmt

# Show detailed graph of resources
terraform graph

# Refresh state
terraform refresh

# Import existing infra
terraform import aws_instance.example i-1234567890abcdef0

# Output variables
terraform output

# Destroy specific resource
terraform destroy -target=aws_instance.example
Project Structure (Suggested)
css
Copy code
.
├── day-01/
│   └── main.tf
├── day-02/
│   ├── variables.tf
│   ├── outputs.tf
│   └── main.tf
├── day-03/
│   ├── backend.tf
│   └── main.tf
├── modules/
│   └── vpc/
│       ├── main.tf
│       ├── variables.tf
│       └── outputs.tf
└── README.md
Docs & Resources
🔗 Terraform CLI Docs

🔗 Terraform Registry

🔗 HashiCorp Learn Tutorials

🔗 Best Practices

