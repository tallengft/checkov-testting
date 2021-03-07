# checkov-testting

# Run Terraform
```bash
cd terraform
terraform init
az login

terraform plan -out=plan
terraform show -json plan > plan.json
checkov -f plan.json
```