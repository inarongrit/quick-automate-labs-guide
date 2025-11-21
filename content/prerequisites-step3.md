# Step 3: Configure Your Environment

Set up your development environment and credentials.

## Configuration Steps

### 1. Configure AWS Credentials

Run the AWS configure command:

```bash
aws configure
```

You'll be prompted to enter:
- AWS Access Key ID
- AWS Secret Access Key
- Default region name (e.g., us-east-1)
- Default output format (json)

### 2. Set Default Region

Ensure your default region is set appropriately for this workshop:

```bash
export AWS_DEFAULT_REGION=us-east-1
```

### 3. Verify Access

Test access to required AWS services:

```bash
# Test S3 access
aws s3 ls

# Test IAM access
aws iam get-user
```

## Environment Variables

You may need to set additional environment variables:

```bash
export AWS_REGION=us-east-1
export AWS_PROFILE=default
```

## Ready to Start

Once you've completed all configuration steps, you're ready to begin the workshop!
