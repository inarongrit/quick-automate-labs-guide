# Step 1: S3 & Bedrock Access Setup

For this workshop, Amazon Quick Suite - Quick Automate needs to access customer data in a customer owned Amazon S3 bucket, generate the product summary using Amazon Bedrock Service and send the product summary via email.

For that we need to configure the service connectors in Quick Automate. We will need the following role and permissions for the Quick Automate workshop to access Amazon S3 and Amazon Bedrock services.

## Create a S3 bucket in your AWS Account
Create a bucket in your account in the region where you have access to Amazon Quick Suite - Quick Automate. Follow the [Instructions](https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html) in AWS documentation if need be.

- Active AWS account
- IAM user with administrator access or appropriate permissions
- AWS CLI installed and configured


