---

AWS Lambda S3 File Transfer Project

This project sets up an AWS environment using Terraform to automatically transfer files from a source S3 bucket to a destination S3 bucket using an AWS Lambda function.

Project Structure:

- variables.tf - Declaration of variables used in Terraform configurations
- terraform.tfvars - Variable values for Terraform configurations
- main.tf - Main Terraform configuration file defining AWS resources
- output.tf - Output file for the Terraform configurations
- index.zip - Zipped file containing the Lambda function code

Prerequisites:

- AWS Account
- Terraform installed on your system
- Visual Studio Code or any IDE for editing code files
- AWS CLI configured (optional)

Setup Instructions:

Task 1: AWS Management Console Access
1. Sign in to the AWS Management Console.
2. Ensure the region is set to US East (N. Virginia) us-east-1.

Task 2: Visual Studio Code Setup
1. Install and open Visual Studio Code.
2. Set up the Terminal and navigate to the project folder.

Task 3: Terraform Variable Configuration
1. Create variables.tf and terraform.tfvars with necessary AWS credentials and region information.

Task 4: S3 Buckets Configuration
1. Define two S3 buckets in main.tf.

Task 5: IAM Role and Policy
1. Set up an IAM role and policy for Lambda to access S3 buckets in main.tf.

Task 6: Lambda Function
1. Add the Lambda function configuration in main.tf.

Task 7: Lambda Trigger
1. Configure the S3 to Lambda trigger in main.tf.

Task 8: Outputs Configuration
1. Define outputs such as the Lambda ARN in output.tf.

Task 9: Terraform Initialization and Application
1. Initialize Terraform and apply the configurations.

Task 10: AWS Resource Validation
1. Validate the resources created through the AWS Management Console.

Task 11: Lambda Function Testing
1. Test the Lambda function by uploading a file to the source S3 bucket.

Task 12: Resource Cleanup
1. Destroy the Terraform-managed resources when done.

Testing:
To test the setup, upload a file to the source S3 bucket and check if it appears in the destination S3 bucket.

Cleanup:
Run terraform destroy to clean up all resources once testing is complete to avoid unnecessary charges.

Conclusion:
By completing this lab, you've successfully automated file transfers between S3 buckets using AWS Lambda.

End Lab:
Sign out of the AWS account and end the lab session from your dashboard.

For a detailed step-by-step guide, refer to the Lab Steps section in this document.

---