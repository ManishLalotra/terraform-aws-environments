# terraform-aws-environments

> Production Infrastructure as Code reference architecture for AWS featuring VPC, Multi-AZ subnets, security groups, and separated staging/production environments.

> [!NOTE]
> Infrastructure code is provided as a production-style reference implementation and is not executed automatically in this portfolio repository.

## Overview
Demonstrates enterprise AWS infrastructure automation using Terraform. Incorporates modular abstractions for networking, security boundaries, and multi-tier subnets across availability zones, with distinct configuration environments for staging and production.

## Project Structure
```text
terraform-aws-environments/
├── environments/
│   ├── staging/
│   │   ├── main.tf
│   │   ├── variables.tf
│   │   └── terraform.tfvars.example
│   └── production/
│       ├── main.tf
│       ├── variables.tf
│       └── terraform.tfvars.example
├── modules/
│   ├── vpc/
│   └── security-groups/
├── docs/
│   └── architecture.md
└── README.md
```

## Validation & Planning (Reference Commands)
```bash
# Staging Validation
cd environments/staging
terraform init
terraform fmt -check
terraform validate
# Planning (requires AWS credentials)
# terraform plan
```

## Author
**Manish Lalotra**  
Full Stack Developer & DevOps Engineer  
*Full Stack Developer | DevOps Engineer | Cloud & Infrastructure Engineer*

## License
MIT License. See [LICENSE](LICENSE) for details.
