AWS Lambda S3 Replication Project

Overview:
This project creates a system to replicate files from a source S3 bucket to a destination S3 bucket automatically using AWS Lambda. Whenever a new file is uploaded to the source bucket, it triggers a Lambda function that replicates the file to the destination bucket.

Files Description:

variables.tf: Declares variables for AWS credentials and region.
terraform.tfvars: Sets the values for the declared variables.
main.tf: Contains the Terraform configuration for AWS resources including S3 buckets, IAM role, and Lambda function.
output.tf: Defines the output for the Terraform setup, such as the ARN of the Lambda function.
index.zip: The Lambda function code that needs to be uploaded to the task_10119_lambda folder.
Setup Process:

Configure AWS Management Console with the specified region.
Setup Visual Studio Code and open the project folder.
Define AWS credentials and desired region in variables.tf and terraform.tfvars.
Create main.tf with S3 bucket details and Lambda function configuration.
Implement IAM role and policies in main.tf for Lambda function access to S3 buckets.
Set up Lambda function trigger for the source S3 bucket in main.tf.
Use output.tf to retrieve the Lambda function ARN.
Initialize and apply Terraform configurations to create the AWS resources.
Verify the creation of resources in AWS Management Console.
Test the replication by uploading a file to the source bucket and checking the destination bucket.
Destroy the resources using Terraform to prevent further charges.
Testing:
Upload a file to the source S3 bucket and verify its presence in the destination S3 bucket to confirm the setup works as intended.

Cleanup:
Execute 'terraform destroy' to remove all resources and avoid incurring costs.

Conclusion:
The project demonstrates an automated setup for S3 bucket replication using Terraform and AWS Lambda.

End Lab:
Remember to sign out of the AWS account and end your lab session appropriately.

This text provides an overview and step-by-step guide on what the project does and how to set it up, test, and clean up after use.