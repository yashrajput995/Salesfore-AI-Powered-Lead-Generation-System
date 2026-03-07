# Role Hierarchy Configuration
## AI-Powered Lead Generation System

## 1. Overview

Role hierarchy in Salesforce controls record-level access and determines how users can view records owned by other users. Users higher in the hierarchy automatically gain access to records owned by users below them.

In the AI-Powered Lead Generation System, role hierarchy was implemented to manage visibility of lead records and ensure proper access control for sales teams.

---

## 2. Purpose of Role Hierarchy

Role hierarchy helps:

- Control record visibility
- Support organizational structure
- Allow managers to access records of their team
- Improve data security and collaboration

---

## 3. Accessing Role Hierarchy

Steps:

1. Login to Salesforce.
2. Click the **Gear Icon (⚙️)**.
3. Click **Setup**.
4. In **Quick Find**, search **Roles**.
5. Click **Roles**.

The Role Hierarchy page displays all roles in a tree structure.

---

## 4. Creating a New Role

Steps:

1. Click **Add Role**.
2. Enter role details.

Example configuration used in this project:

| Field | Value |
|------|------|
| Role Label | AI Sales Executive |
| Role Name | AI_Sales_Executive |
| Reports To | CEO |
| Description | Responsible for managing leads and AI-generated insights |

3. Click **Save**.

---

## 5. Assigning Users to a Role

Steps:

1. Open the role **AI Sales Executive**.
2. Scroll to **Users in This Role**.
3. Click **Add User to Role**.
4. Select the user:


AI Sales


5. Click **Add**.
6. Click **Save**.

---

## 6. Role Hierarchy Structure

The role hierarchy used in this project:


CEO
↓
AI Sales Executive
↓
AI Sales (User)


This structure ensures that higher-level users can access records owned by users below them.

---

## 7. Benefits of Role Hierarchy

Role hierarchy provides several advantages:

- Improves record visibility control
- Supports team-based data access
- Enhances system security
- Allows managers to monitor sales activities
- Enables structured data sharing

---

## 8. Summary

Role hierarchy is an essential part of Salesforce security and access management. In the AI-Powered Lead Generation System, roles were configured to allow structured access to lead records while maintaining secure and organized data visibility across the organization.