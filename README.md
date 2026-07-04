# AWS Infrastructure with Terraform

Provisioned a complete AWS infrastructure stack using Terraform (IaC).

## Resources Created
- **VPC** - Custom VPC with DNS support enabled
- **Public Subnet** - Public subnet in us-east-1a
- **Internet Gateway** - For public internet access
- **Route Table** - Public route table with internet gateway
- **Security Group** - Allow SSH (22) and HTTP (80) inbound
- **EC2 Instance** - t2.micro web server (Amazon Linux 2)
- **S3 Bucket** - Private bucket with public access blocked
- **IAM Role + Policy** - EC2 role with S3 read/write access
- **IAM Instance Profile** - Attached to EC2 instance

## Tools Used
- Terraform v1.14.3
- AWS CLI v2
- AWS Free Tier (us-east-1)

## How to Deploy
```bash
terraform init
terraform plan
terraform apply
```
