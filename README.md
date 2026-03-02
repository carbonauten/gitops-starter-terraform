# gitops-starter-terraform

Standalone Terraform configuration extracted from the `gitops-starter` repository.

Contains multi-cloud infrastructure scaffolding for:

- Azure: resource group, VNet, VPN gateway, Data Lake (ADLS Gen2)
- Alibaba Cloud: VPC, VPN gateway, security group, OSS-based data lake
- Outputs that describe VPN gateways, VNet/VPC IDs, and data lake endpoints.

To use:

```bash
cd gitops-starter-terraform
terraform init
terraform plan
terraform apply
```

Make sure to set/override the variables defined in `variables.tf` (e.g. subscription IDs, regions, CIDRs, and credentials) before applying.

