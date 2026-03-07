# Users Configuration
## AI-Powered Lead Generation System

## 1. Overview
Users in Salesforce represent individuals who can log in to the system and perform actions based on their assigned permissions. Each user is assigned a **profile**, and optionally a **role**, which controls access to objects, records, and system features.

In the AI-Powered Lead Generation System, users were created to allow different roles such as administrators and sales representatives to access and manage lead data securely.

---

## 2. Purpose of User Management

User management ensures that:

- Only authorized individuals can access the Salesforce system
- Each user has appropriate permissions through profiles
- Record visibility can be controlled through role hierarchy
- System access can be monitored and managed

---

## 3. Accessing Users in Salesforce

### Step 1: Access Setup

1. Log in to Salesforce.
2. Click the **Gear Icon (⚙️)** in the top-right corner.
3. Select **Setup**.

---

### Step 2: Navigate to Users

1. In the **Quick Find** search box, type **Users**.
2. Under the **Users** section, click **Users**.

The Users page displays all users in the Salesforce organization, including:

- Active users
- Inactive users
- Frozen users

---

## 4. Creating a New User

Steps to create a user:

1. Click **New User**.
2. Enter the required information.

Example configuration used in this project:

| Field | Value |
|------|------|
| First Name | AI |
| Last Name | Sales |
| Alias | asale |
| Email | yashrajsinghchouhan20@gmail.com |
| Username | aisales2026@gmail.com.dev |
| Nickname | aisales |
| Role | AI Sales Executive |
| User License | Salesforce |
| Profile | AI Sales User |
| Address | Bhopal, Madhya Pradesh, India |
| Time Zone | (GMT+05:30) India Standard Time |
| Language | English |

Additional settings configured:

- **Active**: Checked  
- **Salesforce CRM Content User**: Checked  
- **Receive Salesforce CRM Content Email Alerts**: Checked  
- **Receive Salesforce CRM Content Alerts as Daily Digest**: Checked  
- **Load Lightning Pages While Scrolling**: Checked  

3. Click **Save**.

After saving, Salesforce sends a login email to the user so they can access the system.

This user represents a **Sales Executive role** responsible for managing leads, viewing AI-generated summaries, and interacting with the AI-Powered Lead Generation System.

## 5. Editing an Existing User

To modify an existing user:

1. Go to **Setup → Users → Users**.
2. Click **Edit** next to the user.
3. Update required information such as:

- Profile
- Role
- Email
- Time Zone
- Active Status

4. Click **Save**.

---

## 6. Activating or Deactivating a User

### Deactivating a User

Steps:

1. Click **Edit** next to the user.
2. Uncheck the **Active** checkbox.
3. Click **Save**.

This prevents the user from logging in to Salesforce.

---

### Freezing a User

Freezing a user temporarily blocks login without deleting the account.

Steps:

1. Go to **Setup → Users**.
2. Click the **Freeze** button next to the user name.

---

## 7. Resetting User Password

Steps:

1. Go to **Setup → Users**.
2. Click **Reset Password** next to the user.
3. Salesforce sends a password reset email to the user.

---

## 8. Assigning Permission Sets

Permission sets provide additional permissions beyond profiles.

Steps:

1. Open the **User record**.
2. Scroll to **Permission Set Assignments**.
3. Click **Edit Assignments**.
4. Select the permission sets to assign.
5. Click **Save**.

Permission sets allow administrators to grant additional access without modifying profiles.

---

## 9. Benefits of User Management

Proper user configuration provides several advantages:

- Enhances system security
- Controls access to sensitive data
- Supports role-based access control
- Improves system accountability
- Allows flexible permission management

---

## 10. Summary

User management is an essential component of Salesforce administration. In the AI-Powered Lead Generation System, users were created and configured with appropriate profiles and roles to ensure secure and efficient access to lead data and AI-generated insights.