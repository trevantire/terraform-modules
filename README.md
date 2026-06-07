# Terraform Modules

Reusable Terraform modules for AWS infrastructure.

## Modules
- `vpc/` — Multi-AZ VPC with public/private subnets
- `ecs/` — ECS cluster with auto-scaling
- `rds/` — RDS PostgreSQL with read replicas
- `monitoring/` — CloudWatch alarms + SNS

## Usage
```hcl
module "vpc" {
  source  = "./modules/vpc"
  cidr    = "10.0.0.0/16"
  azs     = ["us-east-1a", "us-east-1b"]
}
```
