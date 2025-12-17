# Step 1: S3 & IAM Access Setup

For this workshop, Amazon Quick Suite - Quick Automate will extract the contents from Public Information from the specific websites, and put the content in spreadsheet format, then upload the file in a customer owned Amazon S3 bucket, generate the product summary using Amazon Bedrock Service and send the product summary via email.

For that we need to configure the service connectors in Quick Automate. We will need the following role and permissions for the Quick Automate workshop to access Amazon S3 and Amazon Bedrock services.

## Create a S3 bucket in your AWS Account
Create a bucket in your account in the region where you have access to Amazon Quick Suite - Quick Automate. Follow the [Instructions](https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html) in AWS documentation if need be.

- Go to the AWS Management Console, Navigate to the **S3 service**
![S3 Service](images/aws-console-s3.png)

- Click **"Create bucket"**, Enter a unique bucket name (must be globally unique across all AWS accounts) e.g. **quick-automate-**<*ACCOUNT-ID*>. *Change ACCOUNT-ID with your AWS Account number*.

- Leave the default setting remain the same. Review all settings, Click **"Create bucket"** button.
- This is what you will get. 
![Create new S3 bucket](images/s3-bucket.png)

## Setup Quick Suite - S3 Permission
- In Amazon Quick Suite that you are successfully authenticated, in the same browser go to the Amazon Quick Suite Admin Console on another page/tab using [Admin](https://us-east-1.quicksight.aws.amazon.com/sn/console/admin?wf=qbs_admin:T1#/landing)

![Quick Suite Resource Permission](images/quick-suite-aws-resources-permission.png)

- Go to the Permissions section in the left hand pane and go to **AWS resources**
- On the Quick Suite access to AWS services page, click on **Amazon S3** check box and choose the S3 bucket that you created earlier with **Write permission for Athena Workgroup** for write permission.

![Quick Suite S3 Access](images/quick-suite-s3-access.png)
![Quick Suite S3 Access](images/quick-suite-s3-access-2.png)

- Click **Save** button to save the permission.

## IAM Role ARN
- Next, Navigate to the **IAM service**
![IAM Service](images/aws-console-iam.png)

- Go to **Roles** under Access Management menu on the left hand side menu. Do a search for **WSParticipantRole** IAM role. 
![IAM Role](images/iam-role-WSParticipantRole.png)

- You will see the Role ARN, take note and do a copy that particular ARN
![IAM Role](images/iam-role-WSParticipantRole-arn.png)

- Repeat the same step, do a search for **aws-quicksight-service-role-v0** IAM role.

- Take a note and copy ARN for **aws-quicksight-service-role-v0** role.
![IAM Role 2](images/iam-role-WSParticipantRole-arn-2.png)

