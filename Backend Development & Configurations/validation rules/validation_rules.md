# Validation Rules
## AI-Powered Lead Generation System

## 1. Overview
Validation rules in Salesforce ensure that the data entered by users meets specific conditions before a record is saved. They help maintain data quality and prevent incorrect or unwanted information from being stored in the system.

In the AI-Powered Lead Generation System, a validation rule was created to prevent users from entering personal email addresses when creating lead records.

---

## 2. Purpose of the Validation Rule

The validation rule ensures that only **business email addresses** are used for lead records. Personal email domains such as Gmail, Yahoo, Hotmail, and Outlook are restricted because they may not represent professional or organizational contacts.

This helps improve the accuracy and reliability of lead data for sales teams.

---

## 3. Validation Rule Details

| Property | Value |
|--------|------|
| Object | Lead |
| Rule Name | Reject_Personal_Email |
| Status | Active |
| Error Location | Email Field |

---

## 4. Error Condition Formula
OR(
CONTAINS(Email,"@gmail."),
CONTAINS(Email,"@yahoo."),
CONTAINS(Email,"@hotmail."),
CONTAINS(Email,"@outlook.")
)
This formula checks the email field for common personal email domains. If the email contains any of these domains, Salesforce will block the record from being saved.

---

## 5. Error Message

When the validation rule is triggered, Salesforce displays the following message:


Personal email domains like Gmail, Yahoo, Hotmail, and Outlook are not allowed.
Please enter a valid business email address.


The error message appears directly below the **Email field** to guide the user in correcting the input.

---

## 6. Steps to Create the Validation Rule

### Step 1: Access Salesforce Setup
1. Log in to your Salesforce Developer Organization.
2. Click the **Gear Icon** in the top-right corner.
3. Select **Setup**.

---

### Step 2: Navigate to Object Manager
1. In the Setup menu, click **Object Manager**.
2. Search for and select the **Lead object**.

---

### Step 3: Open Validation Rules
1. In the left sidebar, click **Validation Rules**.
2. Click **New**.

---

### Step 4: Configure the Validation Rule

Enter the following details:

| Field | Value |
|------|------|
| Rule Name | Reject_Personal_Email |
| Active | Checked |

Insert the error condition formula shown above.

---

### Step 5: Configure Error Message
Enter the following message:


Personal email domains like Gmail, Yahoo, Hotmail, and Outlook are not allowed.


Set the **Error Location** to:

Email Field

---

### Step 6: Save the Rule
Click **Save** to activate the validation rule.

---

## 7. Testing the Validation Rule

To verify that the rule works correctly:

1. Open the **Lead object**.
2. Create a new lead record.
3. Enter an email such as:


test@gmail.com


4. Click **Save**.

Salesforce will display an error message and prevent the record from being saved.

---

## 8. Benefits of Validation Rules

Using validation rules provides several advantages:

- Maintains high data quality
- Prevents invalid or incomplete data entry
- Ensures business rules are enforced
- Improves reliability of CRM data
- Helps sales teams work with accurate lead information

---

## 9. Summary

The **Reject_Personal_Email** validation rule ensures that only professional email addresses are used when creating lead records. This improves the quality of lead data and supports more reliable sales analysis in the AI-Powered Lead Generation System.