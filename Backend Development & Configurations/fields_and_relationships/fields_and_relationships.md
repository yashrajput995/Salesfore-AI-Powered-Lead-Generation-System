# Fields and Relationships
## AI-Powered Lead Generation System

## 1. Overview
Fields and relationships in Salesforce define how data is stored and organized within an object. Custom fields allow administrators to extend the functionality of standard objects by capturing additional information relevant to business processes.

In the **AI-Powered Lead Generation System**, custom fields were created in the **Lead object** to support lead evaluation, categorization, and AI-generated insights. These fields help automate lead management and assist sales teams in prioritizing potential customers.

---

## 2. Custom Fields Created

The following custom fields were created in the **Lead object**:

| Field Label | API Name | Data Type | Description |
|-------------|----------|----------|-------------|
| Lead Score | Lead_Score__c | Number | Stores a numerical score representing the quality or potential value of the lead. |
| Lead Category | Lead_Category__c | Picklist (Hot, Warm, Cold) | Categorizes leads based on their likelihood to convert. |
| Product Interest | Product_Interest__c | Picklist (Training, Consulting, Certification) | Identifies which product or service the lead is interested in. |
| AI Summary | AI_Summary__c | Long Text Area | Stores AI-generated insights and summaries related to the lead. |

These fields help automate lead analysis and support AI-based decision-making within the system.

---

## 3. Steps to Create Custom Fields

### Step 1: Access Salesforce Setup
1. Log in to your Salesforce Developer Organization.
2. Click the **Gear Icon** in the top-right corner.
3. Select **Setup**.

---

### Step 2: Open Object Manager
1. In the Setup menu, click **Object Manager**.
2. The Object Manager displays all standard and custom objects available in Salesforce.

---

### Step 3: Select the Lead Object
1. Search for **Lead** in the Object Manager search bar.
2. Click on **Lead** to open its configuration page.

---

### Step 4: Navigate to Fields & Relationships
1. In the left sidebar, click **Fields & Relationships**.
2. This page displays all existing fields within the Lead object.

---

### Step 5: Create a New Custom Field
1. Click the **New** button.
2. Select the appropriate **Data Type**.
3. Click **Next**.

---

## 4. Example: Creating the AI Summary Field

### Field Configuration

| Property | Value |
|--------|-------|
| Field Label | AI Summary |
| API Name | AI_Summary__c |
| Data Type | Long Text Area |
| Length | 32,768 characters |
| Visible Lines | 5–10 |

Steps:
1. Select **Long Text Area** as the field type.
2. Click **Next**.
3. Enter the field label and verify the API name.
4. Set the length and visible lines.
5. Click **Next**.

---

### Step 6: Configure Field-Level Security
Field-level security determines which profiles can view or edit the field.

Example configuration:

| Profile | Visibility |
|--------|-----------|
| System Administrator | Visible & Editable |
| AI Sales User | Visible |
| Standard User | Visible |

This ensures that only authorized users can access or modify sensitive information.

---

### Step 7: Add Field to Page Layout
1. Select the **page layouts** where the field should appear.
2. Click **Save**.

Once saved, the field will appear on the **Lead record page**.

---

## 5. Creating Other Custom Fields

The same steps were repeated to create the remaining fields.

### Lead Score Field

| Property | Value |
|--------|-------|
| Field Label | Lead Score |
| API Name | Lead_Score__c |
| Data Type | Number |

Purpose:
Stores a numerical value representing the quality or priority of a lead.

---

### Lead Category Field

| Property | Value |
|--------|-------|
| Field Label | Lead Category |
| API Name | Lead_Category__c |
| Data Type | Picklist |

Picklist Values:
- Hot
- Warm
- Cold

Purpose:
Helps categorize leads based on their likelihood of conversion.

---

### Product Interest Field

| Property | Value |
|--------|-------|
| Field Label | Product Interest |
| API Name | Product_Interest__c |
| Data Type | Picklist |

Picklist Values:
- Training
- Consulting
- Certification

Purpose:
Identifies the service or product the lead is interested in.

---

## 6. Benefits of Custom Fields

Creating custom fields provides several advantages:

- Captures additional lead information
- Improves lead qualification process
- Enables automation and AI integration
- Supports advanced reporting and analytics
- Helps sales teams prioritize high-value leads

---

## 7. Summary

The custom fields created in the **Lead object** provide the foundation for the AI-Powered Lead Generation System. These fields allow Salesforce to store lead evaluation data, categorize prospects, and generate AI-powered insights that help sales teams make better decisions.