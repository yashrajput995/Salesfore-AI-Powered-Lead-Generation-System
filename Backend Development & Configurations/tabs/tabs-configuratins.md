# Tabs Configuration
## AI-Powered Lead Generation System

## 1. Overview
Tabs in Salesforce provide quick access to objects, records, and application features. They act as navigation elements within Salesforce apps, enabling users to easily locate and manage data.  

In this project, a **Custom Object Tab** was created for the **AI Lead Prediction** object so that users can directly access AI-generated lead insights from the Salesforce navigation bar.

---

## 2. Steps to Create a Custom Object Tab

### Step 1: Access Salesforce Setup
1. Log in to the Salesforce Developer Organization.
2. Click the **Gear Icon** in the top-right corner.
3. Select **Setup**.

---

### Step 2: Navigate to Tabs Section
1. In the **Quick Find** search bar, type **Tabs**.
2. Under the **User Interface** section, click **Tabs**.

This page lists all types of tabs available in Salesforce, including:
- Standard Tabs
- Custom Object Tabs
- Visualforce Tabs
- Lightning Page Tabs
- Web Tabs

---

### Step 3: Create a New Custom Object Tab
1. Locate the **Custom Object Tabs** section.
2. Click **New**.
3. The **New Custom Object Tab** configuration page will open.

---

### Step 4: Configure Tab Settings

#### A. Select the Custom Object
Choose the object for which the tab will be created.

Example:

| Setting | Value |
|--------|------|
| Object | AI Lead Prediction |

---

#### B. Choose a Tab Style
Select a tab style from the available icons and colors.

Example:
- Icon: Analytics / Chart Icon
- Color: Default Salesforce Theme

The tab style helps visually identify the object in the navigation menu.

---

#### C. Add Additional Information (Optional)
Optional fields may include:

- Description of the tab
- Custom splash page (rarely used)

Example Description:

"This tab provides access to AI-generated lead predictions and insights."

---

### Step 5: Set Tab Visibility for Profiles

Tab visibility determines which user profiles can see the tab.

Options include:

| Option | Meaning |
|------|------|
| Default On | Tab appears automatically in navigation |
| Default Off | Users can manually add the tab |
| Tab Hidden | Tab is not visible for that profile |

Example Configuration:

| Profile | Visibility |
|------|------|
| System Administrator | Default On |
| AI Sales User | Default On |

---

### Step 6: Add Tab to Application

After configuring visibility, Salesforce prompts you to assign the tab to an application.

Example Apps:

- Sales App
- AI Lead Management App

Adding the tab ensures users can access the object directly from the app navigation bar.

---

### Step 7: Verify the Tab

To confirm successful creation:

1. Open the **App Launcher (9-dot icon)**.
2. Search for the custom tab name.
3. Open the tab.
4. Verify that records can be created and viewed.

---

## 3. Purpose of Tabs in the System

The custom tab created for the **AI Lead Prediction** object allows users to:

- Access AI lead analysis records easily
- View and manage prediction data
- Navigate directly to AI insights without using Object Manager

This improves usability and enhances the overall user experience within the Salesforce application.

---

## 4. Benefits

Creating tabs provides several advantages:

- Improves system navigation
- Enhances user productivity
- Provides quick access to important objects
- Organizes the workspace effectively