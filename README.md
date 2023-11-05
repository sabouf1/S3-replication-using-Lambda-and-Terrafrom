# AWS Lambda S3 Replication Project

## Overview
This project automatically replicates files from a source Amazon S3 bucket to a destination S3 bucket using AWS Lambda. When a new file is uploaded to the source bucket, a Lambda function is triggered to replicate the file to the destination bucket.

## Project Structure
- `variables.tf` - Variable declarations for AWS configuration.
- `terraform.tfvars` - Values for the Terraform variables.
- `main.tf` - Terraform configuration for AWS resources.
- `output.tf` - Terraform output definitions.
- `index.zip` - Zipped Lambda function code.

## Prerequisites
- An AWS account
- Terraform installed on your local machine
- Visual Studio Code or another IDE

## Setup Steps
1. **AWS Console Configuration**: Sign in and set the region to US East (N. Virginia) us-east-1.
2. **IDE Setup**: Install and set up Visual Studio Code.
3. **Terraform Variables**: Define AWS credentials in `variables.tf` and `terraform.tfvars`.
4. **S3 Bucket Configuration**: Create S3 bucket details in `main.tf`.
5. **IAM Role and Policy**: Configure IAM role and policy for Lambda S3 access in `main.tf`.
6. **Lambda Function Setup**: Establish Lambda function and triggers in `main.tf`.
7. **Outputs Definition**: Use `output.tf` to define the required outputs like Lambda ARN.
8. **Terraform Initialization**: Run `terraform init` to initialize Terraform.
9. **Apply Configuration**: Execute `terraform apply` to create the AWS resources.

## Testing the Setup
Upload a file to the source S3 bucket and ensure it replicates to the destination S3 bucket.

## Cleanup
Run `terraform destroy` when finished to remove all created resources and avoid unnecessary charges.

## Conclusion
This project sets up a file replication system between two S3 buckets, utilizing AWS Lambda for automation.

## End Lab
Don't forget to sign out of the AWS Management Console when finished with your lab work.
