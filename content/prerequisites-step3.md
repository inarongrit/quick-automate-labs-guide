# Step 3: Configure Amazon Bedrock connector

- Now lets create Amazon Bedrock connector. From the same Amazon Quick Suite Admin console, On the action connectors page, click on the New action button in the top right to create a new action connector

![New Action Button](images/1p-connector-newaction.png)

- Select the 1P connector you want to create. Select Bedrock Runtime for this workshop.

![Bedrock Connector Selection](images/1p-connector-bedrock.png)

- Fill in the details for the name and the role that you created earlier.Provide the Role ARN in the connection details. This will be the role that grants the connector permissions to perform actions on resources.

![Bedrock Connector Details 1](images/1p-connector-bedrock-details-1.png)

![Bedrock Connector Details 2](images/1p-connector-bedrock-details-2.png)

- Share the connector to at least one user or group to share the connector with. Click Share to add the user to the list. Then, select either Owner or User permissions. Click the Add button.

- Owner permissions are recommended if you are granting the connector to your own alias/user. This enables you to share, edit and delete the connector after creation.

![Share Connector](images/1p-connector-share.png)

- After adding the connector, you should be able to view the new connector in the list of Actions on the Amazon QuickSight Console page. Confirm the new connector is part of the list.

![Bedrock Connector List](images/ip-connector-bedrock-list.png)

