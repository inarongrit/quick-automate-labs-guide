# Module 2: Build the Automate Workflow

## Overview
Ok, we are all set to start building a workflow automation using Amazon Quick Suite - Quick Automate!

Creating an AWS Announcements Monitoring Automation in Quick Automate.
This automation will monitor AWS announcements weekly, extract key information, and generate formatted Excel reports stored in S3.

- You can ignore a step below if you continue from previous Section. 
- Navigate to the Amazon Quick Suite, Quick Automate Project and Select the previous project that you just created it earlier. Click **Start Building**  
![Create multi-agent Workflow Automation](../images/create-multi-agent-automation.png)

- You can start with Samples instruction like **Market Analysis AI Assistant**, **Form Filling UI Automation**, **Weather Forecast Agent**, or else to explore the Quick Automat capabilities. However, for this hands-on lab instruction we will use the the prompt below.

- Copy and Paste this instruction prompt in the input box. 

```
Create a weekly automation that monitors AWS announcements from aws.amazon.com/new/ and use LLM to summary the key highlight how it handy from that particular announcement.
Note: Please be mindful when interacting with displayed links and processes them into an Excel report stored in S3. The workflow should:
Schedule: Run every Monday at 9 AM to collect the previous week's announcements
Data Collection: Extract announcement headlines, publication dates, and detailed descriptions from the AWS What's New page
Data Processing: Structure the data with columns for:
- Announcement Date
- Headline/Title
- Service Category (e.g., EC2, S3, Lambda)
- Brief Description
- Full Details/Summary
- Announcement URL
Output: Generate an Excel spreadsheet with formatted data
Storage: Upload the completed Excel file to S3 bucket [quicksuite-automate-{AWS-ACCOUNT-ID}] with filename format 'AWS-Announcements.xlsx'
```

- Then click **Generate**
- Review the automate workflow creation created by Quick Automate
![Automation project workflow Creation](../images/Automation-project-workflow-creation.gif)

