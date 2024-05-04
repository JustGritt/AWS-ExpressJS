# Terraform Deployment Application

This application is designed to automate the process of deploying infrastructure on AWS using Terraform.

## Prerequisites

- Terraform installed on your local machine
- AWS account with necessary permissions

## Setup

0. Export the AWS access key and secret key as environment variables.

```bash
export AWS_ACCESS_KEY_ID="REPLACE_WITH_YOUR_ACCESS_KEY"
export AWS_SECRET_ACCESS_KEY="YOUR_SECRET_ACCESS_KEY"
export AWS_REGION="us-west-2"
```

1. Initialize the Terraform configuration.

```bash
terraform init
```

1. Plan the Terraform configuration to see what resources will be created.

```bash
terraform plan
```

3. Apply the Terraform configuration to create the infrastructure.

```bash
terraform apply
```

** Note: You will be prompted to enter the PEM key name for the EC2 instance.

4. Once the infrastructure is created, the public IP address of the EC2 instance will be displayed in the output. Enjoy and visit the application in your browser `<public-ip>:3000`