# Agentforce Prompt Builder Configuration
## AI-Powered Lead Generation System

## 1. Overview
Salesforce Einstein AI provides intelligent automation features that help organizations generate insights from CRM data. In this project, **Prompt Builder** was used to automatically generate AI-powered summaries for lead records.

The AI-generated summary helps sales representatives quickly understand the background, contact information, and engagement level of a lead.

---

## 2. Prerequisite: Create AI Summary Field

Before creating the prompt template, a custom field was created in the Lead object.

Field configuration:

| Property | Value |
|--------|------|
| Field Label | AI Summary |
| API Name | AI_Summary__c |
| Data Type | Long Text Area |
| Length | 32,000 |
| Visible Lines | 5–10 |

This field stores the AI-generated lead summary.

---

## 3. Enable Einstein AI

Steps:

1. Go to **Setup**.
2. Search **Einstein Setup** in Quick Find.
3. Click **Einstein Setup**.
4. Enable **Turn on Einstein**.
5. Refresh the page.

Enabling Einstein allows access to AI features such as Prompt Builder.

---

## 4. Create Prompt Template

### Step 1: Open Prompt Builder

1. Go to **Setup**.
2. Search **Prompt Builder**.
3. Click **Prompt Builder**.
4. Click **New Prompt Template**.

---

### Step 2: Configure Template

| Field | Value |
|------|------|
| Prompt Type | Field Generation |
| Label | AI Summary Field Generation |
| Object | Lead |
| Field | AI Summary |

This configuration allows AI to generate text and store it directly in the AI Summary field.

---

## 5. Insert Lead Data Resources

The prompt template uses lead record data as input.

Resources used:

- {!Lead.FirstName}
- {!Lead.LastName}
- {!Lead.Company}
- {!Lead.Email}
- {!Lead.Phone}
- {!Lead.LeadSource}
- {!Lead.Status}
- {!Lead.Description}

These fields provide context to the AI model.

---

## 6. Prompt Template

The following prompt was used to generate lead summaries:


Generate a detailed summary of this Lead using the selected fields.

Explain the Lead’s background, company information, contact details, status, source, and any key notes clearly.

Summarize relevant details such as the current engagement stage, potential interest level, communication history, and any important remarks.

Provide the summary in a clean, structured, and easy-to-understand format.


---

## 7. Save and Activate Template

Steps:

1. Click **Save**.
2. Click **Activate**.

The prompt template is now available for use within Salesforce.

---

## 8. Deploy Prompt Template to Lead Page

To enable AI summary generation directly on the Lead page:

1. Open any **Lead record**.
2. Click the **Gear Icon → Edit Page**.
3. Upgrade the layout to **Dynamic Forms**.
4. Select the **AI Summary field**.
5. In the right-side panel, assign the prompt template:


AI Summary Field Generation


6. Click **Save**.
7. Click **Activate**.
8. Assign as **Org Default**.

---

## 9. Testing the AI Summary

Steps to test the feature:

1. Open any Lead record.
2. Locate the **AI Summary field**.
3. Click the **AI Stars Icon** next to the field.
4. Click **Use** to generate the summary.
5. Click **Save**.

Salesforce will generate an AI-powered summary based on the lead data.

---

## 10. Benefits of AI Prompt Builder

Using Prompt Builder provides several advantages:

- Automatically generates lead insights
- Reduces manual analysis of lead data
- Improves sales decision-making
- Enhances productivity of sales teams
- Integrates AI directly into Salesforce workflows

---

## 11. Summary

The Prompt Builder configuration enables AI-powered lead analysis within the Salesforce AI-Powered Lead Generation System. By automatically generating summaries of lead information, the system helps sales teams quickly understand potential customers and prioritize high-value opportunities.