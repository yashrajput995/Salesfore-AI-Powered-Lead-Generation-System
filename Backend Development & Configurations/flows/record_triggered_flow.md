# Record-Triggered Flow
## AI-Powered Lead Generation System

## 1. Overview
Salesforce Flow is a powerful automation tool that allows administrators to automate business processes without writing code. In the AI-Powered Lead Generation System, a **Record-Triggered Flow** was created to automatically send an email notification when a new lead is created or updated.

This automation ensures that sales teams receive immediate updates when new leads are generated and when AI-generated summaries are available.

---

## 2. Purpose of the Flow

The Record-Triggered Flow performs the following tasks:

- Automatically triggers when a Lead record is created or updated
- Retrieves information from the Lead record
- Sends an email notification containing AI-generated lead insights
- Helps sales representatives respond quickly to new leads

This automation improves response time and reduces manual communication.

---

## 3. Flow Type

| Property | Value |
|--------|------|
| Flow Type | Record-Triggered Flow |
| Object | Lead |
| Trigger | When a record is created or updated |
| Optimization | Actions and Related Records |
| Run Time | Immediately after record save |

---

## 4. Steps to Create the Flow

### Step 1: Access Flow Builder
1. Log in to Salesforce.
2. Click the **Gear Icon (⚙️)**.
3. Select **Setup**.
4. In the **Quick Find** search box, type **Flows**.
5. Click **Flows**.

---

### Step 2: Create a New Flow
1. Click **New Flow**.
2. Select **Triggered Flow**.
3. Choose **Record-Triggered Flow**.
4. Click **Create**.

---

### Step 3: Configure the Start Element

| Setting | Value |
|------|------|
| Object | Lead |
| Trigger | A record is created or updated |
| Optimize Flow For | Actions and Related Records |
| When to Run | Run Immediately |

Click **Done**.

---

## 5. Add Send Email Action

To automate email notifications:

1. Click the **+ icon** below the Start element.
2. Select **Action**.
3. Search for **Send Email**.
4. Select the **Send Email** action.

---

## 6. Configure Email Action

| Field | Value |
|------|------|
| Label | Send Lead Email |
| Subject | New Lead Notification - AI Summary Available |
| Recipient Addresses | {!$Record.Email} |
| Sender Type | Current User |
| Rich Text Body | Enabled |

---

## 7. Email Body Template

The email body contains lead information and AI-generated insights.


Hello,

A new lead has been processed by the AI Lead Management System.

Lead Name: {!$Record.FirstName} {!$Record.LastName}
Email: {!$Record.Email}
Lead Score: {!$Record.Lead_Score__c}
Lead Category: {!$Record.Lead_Category__c}

AI Summary:
{!$Record.AI_Summary__c}

Please review this lead and take necessary action.

Thank You.


---

## 8. Activate the Flow

After configuring the action:

1. Click **Done**
2. Click **Save**
3. Enter Flow Name:


Lead_Email_Notification_Flow


4. Click **Activate**

Once activated, the flow will automatically trigger whenever a lead record is created or updated.

---

## 9. Flow Logic Diagram

Lead Record Created/Updated  
↓  
Record-Triggered Flow  
↓  
Retrieve Lead Data  
↓  
Send Email Notification  
↓  
Sales Team Receives Lead Details

---

## 10. Benefits of Flow Automation

Using Salesforce Flow provides several advantages:

- Automates repetitive processes
- Reduces manual work
- Improves response time for sales teams
- Ensures consistent communication
- Integrates with AI-generated lead insights

---

## 11. Summary

The Record-Triggered Flow automates email notifications whenever a new lead is created or updated in the system. By combining Salesforce automation with AI-generated summaries, the system ensures that sales representatives receive timely information about potential leads, enabling faster and more effective decision-making.