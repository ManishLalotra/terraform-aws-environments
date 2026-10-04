# Terraform AWS Multi-Environment Blueprint

> Infrastructure code is provided as a production-style reference implementation and is not executed automatically in this portfolio repository.

## Design Highlights
- **Environment Isolation**: Distinct state files and parameter sets for Staging and Production.
- **VPC Subnetting**: Multi-AZ tiering separating public ingress subnets from isolated private application/database subnets.
- **Least Privilege Security Groups**: Explicit port mapping between Application Load Balancers and compute clusters.
