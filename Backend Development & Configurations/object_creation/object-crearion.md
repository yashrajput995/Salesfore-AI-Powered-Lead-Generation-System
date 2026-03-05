# Custom Object Creation
## AI-Powered Lead Generation System

## 1. Overview
In the Salesforce AI-Powered Lead Generation System, custom objects are created to store and manage specific data related to the application. Custom objects allow administrators to define their own database structure within Salesforce.

---

## 2. Steps to Create a Custom Object

### Step 1: Access Salesforce Setup
1. Log in to your Salesforce Developer Organization.
2. Click the **Gear Icon** in the top-right corner.
3. Select **Setup**.

---

### Step 2: Navigate to Object Manager
1. In the Setup menu, click **Object Manager**.
2. The Object Manager displays all standard and custom objects in Salesforce.

---

### Step 3: Create a New Custom Object
1. Click **Create → Custom Object**.
2. The Custom Object Definition page will open.

---

### Step 4: Configure Custom Object Details

Fill the following details:

| Field | Value |
|------|------|
| Label | AI Lead Prediction |
| Plural Label | AI Lead Predictions |
| Record Name | Prediction ID |
| Data Type | Auto Number |
| Display Format | PRED-{0000} |

Optional Features Enabled:

- Allow Reports
- Allow Activities
- Track Field History
- Allow Search
- Allow Notes & Attachments

Deployment Status:

- Deployed

---

### Step 5: Set Object-Level Security

Enable the following permissions:

- Allow Sharing
- Enable Reports
- Allow Bulk API Access
- Allow Activities

These settings allow users to interact with the object securely.

---

### Step 6: Save the Custom Object

Click **Save**.

The new custom object will appear in the **Object Manager** and can now be used to store lead-related prediction data in the AI-Powered Lead Generation System.

---

## 3. Purpose of the Custom Object

The **AI Lead Prediction** object is used to store and manage AI-generated insights about potential leads. It helps sales teams analyze lead behavior and prioritize prospects more efficiently.