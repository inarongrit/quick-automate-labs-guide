# Step 2: Configure Amazon S3 connector

- Now that you are successfully authenticated, in the same browser go to the Amazon Quick Suite Admin Console on another page/tab using [Admin](https://us-west-2.quicksight.aws.amazon.com/sn/console/admin?wf=qbs_admin:T1#/landing)

![Admin Console](images/1p-connector-admin.png)

- Go to the Permissions section in the left hand pane and go to **AWS actions**
- On the action connectors page, click on the **New action** button in the top right to create a new action.

![New Action Button](images/1p-connector-newaction.png)

- Select the S3 connector you want to create for this workshop.

![S3 Connector Selection](images/1p-connector-s3.png)

- Fill in the details for the name and the role that you created earlier.Provide the Role ARN in the connection details. This will be the role that grants the connector permissions to perform actions on resources.

![S3 Connector Details 1](images/1p-connector-s3-details-1.png)

![S3 Connector Details 2](images/1p-connector-s3-details-2.png)

- Share the connector to at least one user or group to share the connector with. Click Share to add the user to the list. Then, select either Owner or User permissions. Click the Add button.

- Owner permissions are recommended if you are granting the connector to your own alias/user. This enables you to share, edit and delete the connector after creation.

![Share Connector](images/1p-connector-share.png)

- After adding the connector, you should be able to view the new connector in the list of Actions on the Amazon QuickSight Console page. Confirm the new connector is part of the list.

![S3 Connector List](images/ip-connector-s3-list.png)

