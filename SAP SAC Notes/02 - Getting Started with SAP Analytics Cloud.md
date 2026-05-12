# 📊 SAP Analytics Cloud — Navigation, Files & My Metrics

> A detailed reference guide for navigating SAP Analytics Cloud, managing files, sharing content, and working with My Metrics dashboards.


---

## 📚 Table of Contents

1. [Home Screen](#1--home-screen)
2. [Navigation Elements](#2--navigation-elements)
3. [Profile & Settings](#3--profile--settings)
4. [Catalog](#4--catalog)
5. [Themes](#5--themes)
6. [Managing Files](#6--managing-files)
7. [Sharing Files](#7--sharing-files)
8. [Scheduling Publications](#8--scheduling-publications)
9. [Content Network](#9--content-network)
10. [Security & Monitoring](#10--security--monitoring)
11. [My Metrics](#11--my-metrics)
12. [Smart Insights](#12--smart-insights)
13. [Quick Summary](#13--quick-summary)

---

## 1. 🏠 Home Screen

When you first log in to your SAP Analytics Cloud **tenant**, you are automatically directed to the **Home Screen**. This is your personal starting point — it displays your recent stories and visualizations as interactive cards.

> 🔒 **Privacy Note:** Your home screen is completely **private**. You cannot share it with other users or add it to discussions. This privacy also applies to any notes and cards you pin there.

### Home Screen Tabs

The home screen is divided into **four tabs**:

| Tab | Description | Notes |
|-----|-------------|-------|
| **Today** | Default tab — contains your pinned cards and notes | Fully private and personal |
| **Catalog** | Single access point for all content published for users | View-only; managed by admins |
| **Favorites** | Lists all resources you have marked as favorites | Quick access to preferred content |
| **Shared With Me** | Lists all resources that other users have shared with you | Reflects shared access permissions |

> ⚠️ **Admin Note:** The **Catalog**, **Favorites**, and **Shared With Me** tabs can be **disabled** by an administrator or a user with the necessary permissions.

### Customizing the Home Screen

You can personalize your home screen to match your workflow:

1. Select **Customize** from the home screen, **or**
2. Go to **Profile → Settings → Home Screen**

From there you can:
- ✅ Change the **default tab** that opens on login
- ✅ **Add** new cards to your home screen
- ✅ **Resize** existing cards
- ✅ **Remove** cards you no longer need

> Simply toggle the selector **on** or **off** for each card option.

---

## 2. 🧭 Navigation Elements

SAP Analytics Cloud has two primary navigation components that are always visible throughout the interface.

### Shell Bar *(Top of Screen)*

The **shell bar** is the uppermost horizontal section of the interface. It is divided into two sides:

| Side | Elements | Purpose |
|------|----------|---------|
| **Left** | Breadcrumb navigation | Shows your current location in the folder path; click any part to jump to that level |
| **Right** | Search 🔍 · Notifications 🔔 · Help ❓ · Profile 👤 | Universal actions accessible from anywhere in the app |

**Shell Bar Actions Explained:**

- **🔍 Search** — Search for stories, models, and other content across your tenant
- **🔔 Notifications** — View alerts and updates from the system
- **❓ Help** — Opens in-application contextual help based on where you currently are
- **👤 Profile** — Access your user settings and preferences

### Side Navigation *(Left Panel)*

The **side navigation** panel appears on the left side of the interface and provides quick access to all major SAP Analytics Cloud applications and sections.

- Always accessible from any screen
- Allows fast switching between different apps (Stories, Models, Planning, etc.)
- Collapses to icons for a wider workspace view

### Help Feature

SAP Analytics Cloud has a robust **embedded help system**:

- Click the **Help icon** in the shell bar for context-sensitive help
- Includes **guided tutorials**, **videos**, and **help documents**
- You can also search the full **SAP Help Portal** documentation directly from the home screen
- To exit help, click the Help icon again

---

## 3. 👤 Profile & Settings

Your user profile is used throughout SAP Analytics Cloud to identify you and personalize your experience.

### Accessing Your Profile

Click the **Profile icon** in the top-right of the shell bar to access your settings.

### Where Profiles Appear in SAP Analytics Cloud

Your profile — including your photo and display name — appears in multiple places:

| Location | How Profile Appears |
|----------|-------------------|
| **Collaboration Panel** | Name and picture of every discussion participant; hover to view full profile or start a 1-on-1 discussion |
| **Calendar Events** | Profile picture of the user assigned to an event or task |
| **User Management** | Full profile displayed by clicking the user's ID |
| **User Selection Dialogs** | Picture, display name, and ID shown together |

### Profile Settings Options

Access all preferences via **Profile → Settings**:

#### 🖼️ Profile Picture
- A photo placeholder is shown by default
- To upload a picture: go to **User Account settings** and select the placeholder
- To change your picture: click the **Edit icon**

#### 🌐 Language & Region

| Setting | Description |
|---------|-------------|
| **Display Language** | The language used for the SAP Analytics Cloud interface |
| **Data Access Language** | Language used for displaying live data and text in stories; defaults to Display Language if set to "Default" |
| **Date Format** | Customize how dates appear across the interface |
| **Number Format** | Customize decimal separators, thousand separators, etc. |
| **Currency Position** | Set whether currency symbols appear before or after values |

> 📌 **Note:** When you send a model for translation, the **Data Access Language** becomes the **source language** of the model.

---

## 4. 📂 Catalog

The **Catalog** is a centralized, read-only content library that gives all users a single access point to browse and discover published content within SAP Analytics Cloud.

### Key Characteristics

- Each published item is displayed as a **tile/card**
- Content is **view-only** — you cannot copy, paste, delete, or edit anything in the catalog
- Supports **search and filtering by category** to find content quickly

### Content Types Published to the Catalog

The following types of content can be published and displayed:

| Content Type | Description |
|-------------|-------------|
| **Stories** | Interactive reports and dashboards |
| **Digital Boardroom Presentations** | Executive-level presentation views |
| **Models** | Business data models used as the basis for stories |
| **Datasets** | Raw or processed datasets |
| **Uploaded SAP Analytics Cloud Files** | Files imported into the system |
| **Content Links** | Links to external or related content |

### How Admins Publish to the Catalog

> 🔑 Publishing to the catalog is an **administrative function only**.

Steps for an administrator to publish content:
1. Select the object from **Files**
2. Choose **Share → Publish to Catalog**
3. Select the **team** to share with and choose **OK**
4. Choose **Share**

---

## 5. 🎨 Themes

SAP Analytics Cloud supports the modern **SAP Horizon** design system with four available themes:

| Theme | Style | Best For |
|-------|-------|---------|
| **SAP Morning Horizon** | Light mode | Standard daytime use |
| **SAP Evening Horizon** | Dark mode | Low-light environments |
| **SAP Horizon High Contrast Light** | High contrast on light background | Accessibility needs |
| **SAP Horizon High Contrast Dark** | High contrast on dark background | Accessibility needs |

> 💡 Change your theme anytime from **Profile → Settings**. During the transition period, the legacy **SAP Belize** theme is also available.

---

## 6. 📁 Managing Files

The **Files** area is the central repository where all SAP Analytics Cloud resources are stored and managed.

### My Files — Folder Structure

All users have access to the **My Files** area, which includes:

| Folder | Description | Permissions |
|--------|-------------|-------------|
| **My Files (root)** | Content you own + content shared with you | Full control over your own content |
| **Input Forms** | Planning stories and planning-related elements assigned to you | Assigned by admins/planners |
| **Public** | Content available to all users | Read-only for other users by default |
| **Samples** | Example models and stories provided by SAP | For learning and reference |

### Working with Files

- **Click a filename** → Opens the file directly
- **Check the checkbox** next to a file → Reveals additional file options in the **file ribbon**
- From the file ribbon you can: share, move, copy, delete, schedule, and more

### Public Folder Rules

- Content saved in the Public folder is **read-only for other users by default**
- The Public folder **cannot be deleted or copied**
- Administrators can assign **copy and delete permissions** to the Public folder
- Items created in the Public folder **inherit** the folder's sharing permissions

---

## 7. 🔗 Sharing Files

SAP Analytics Cloud allows flexible content sharing using **Access Levels** — predefined groups of permissions that make it easy for admins to manage access across teams.

### Access Levels

> Each level (except Custom) **includes all permissions from the level above it**.

| Access Level | Permissions Included |
|-------------|---------------------|
| **View** | Read · Copy · View comment · Add comment |
| **Edit** | Update · Create files · Create folders *(+ all View permissions)* |
| **Full Control** | Delete · Delete comment · Share *(+ all Edit permissions)* |
| **Custom** | Any combination of individual permissions you configure |

### How to Share a File

**Method 1 — From Files Area:**
1. Check the **checkbox** next to the filename(s) *(supports multiple files)*
2. Click the **Share icon**
3. Choose **Share**

**Method 2 — From Inside an Opened File:**
1. Click the **Share icon** within the file
2. Choose **Share**

**In the Share Dialog:**
1. Add the **users or teams** you want to share with
2. Choose the appropriate **access level**
3. *(Optional)* Check **"Email new recipients"** to notify them
4. Click **Share**

### How to Unshare a File

1. Open the **Share dialog** for the file
2. In the **Shared With** area, select the relevant users or teams
3. Click **Delete**

### Featured Files

Administrators can make important content more visible by:
- Adding a **Featured Files card** to users' Home screens
- Sharing key files directly to this featured card for easy discovery

---

## 8. 📅 Scheduling Publications

As a **content owner**, you can automate the distribution of stories by scheduling them to be shared on a regular basis.

### Scheduling Rules

| Rule | Detail |
|------|--------|
| **SAP Analytics Cloud Users** | Unlimited number within the tenant |
| **Non-SAP Users** | Maximum of **3 external recipients** |
| **Required Privilege** | Must have **Schedule Publication** privileges (Create and Manage) |

### Scheduling Steps *(General Flow)*

1. Open the story you want to schedule
2. Access the **Schedule Publication** option
3. Configure the recipients, frequency, and format
4. Save and activate the schedule

> The story will be automatically shared at the configured intervals without any manual action needed.

---

## 9. 🌐 Content Network

The **Content Network** is an administrative feature used to promote and transfer content between multiple SAP Analytics Cloud tenants (e.g., from Development to Production).

### Key Features

| Feature | Detail |
|---------|--------|
| **Content Transfer** | Move content across tenants via the cloud |
| **Access Control** | Admins set different access rights per sharing destination |
| **Free Storage** | Up to **300 MB** of exported content stored free in My Content area |
| **SAP Business Content** | Stored here; admins can import and make it available to users |

### Content Network Includes

- All **files** (stories, models, datasets)
- **Planning-related objects** (data actions, value driver trees)

---

## 10. 🔒 Security & Monitoring

SAP Analytics Cloud has a comprehensive security and audit framework managed by system administrators.

### Security Model

- Defines access for both **functional** (what you can do) and **data** (what you can see) levels
- Typically created and controlled by **corporate SAP Analytics Cloud administrators**

### Audit Logging

- SAC **logs all user activities** performed in the system
- Administrators can access and review these audited activities from the **Security area**
- Standard **monitoring reports** are available to track real-time statistics and system usage

### Release & Versioning Rules

> ⚠️ Important rules to follow when managing multiple tenants:

- SAP Analytics Cloud follows a **quarterly release cycle**
- Source and target tenants must have the **same version** or differ by **only one version**
- There is **no backward compatibility** between versions that differ by more than one release

---

## 11. 📊 My Metrics

**My Metrics** is a personalized, real-time KPI watchlist that consolidates your most important business metrics into a **single screen** — eliminating the need to open multiple dashboards or reports.

> 💡 Think of it as your personal **command center** for monitoring business performance at a glance.

### The 3 Areas of My Metrics

```
┌──────────────────────┐     ┌──────────────────────┐     ┌──────────────────────┐
│                      │     │                      │     │                      │
│    Your Metrics      │ ──► │  Detailed            │ ──► │   Smart Insights     │
│                      │     │  Visualization       │     │                      │
│  Collection of all   │     │  Chart view of the   │     │  AI-powered auto-    │
│  metric cards you    │     │  selected metric     │     │  matic analysis of   │
│  created or received │     │  with applied        │     │  patterns and trends │
│                      │     │  filters             │     │                      │
└──────────────────────┘     └──────────────────────┘     └──────────────────────┘
```

### Metrics List Options

From the **More Settings (⋮)** menu on a metrics list, you can:

| Option | Description |
|--------|-------------|
| **Rename** | Update the name of the list |
| **Reload** | Refresh the list to display the latest data updates |
| **Share** | Share the entire list with stakeholders (View / Edit / Full Control) |
| **Show Difference As** | Toggle between displaying change as a **percentage** or **absolute value** |
| **Delete Metrics List** | Permanently delete the entire list |

> 🔃 You can **sort** cards by: Recently Added · A-Z · Z-A

### Individual Metric Card Options

For each metric **card** within a list, you can:

| Option | Description |
|--------|-------------|
| **Rename** | Update the metric's display name |
| **Move Up / Move Down** | Reorder cards manually; also supports **drag and drop** |
| **Share** | Share the individual metric (View / Edit / Full Control); auto-saved to recipient's *Individually Shared Metrics* list |
| **Jump to Original** | Open the source story in current or new browser tab |
| **Move To** | Move the metric to a different list or create a new list |
| **Copy To** | Copy a metric to multiple lists if relevant in more than one context |
| **Smart Insights** | Open the AI-powered Smart Insights analysis for this metric |
| **Delete from Metrics List** | Permanently removes the metric from the list; can be done by the owner or a user with Full Control |

### Key Behaviors

- Selecting a card → Data is **instantly visualized** in the Detailed Visualization area
- The **chart type** is set when the metric is first created
- **Filters** applied to the metric are displayed alongside the visualization
- **Smart Insights** can be toggled on or off per metric

---

## 12. 🤖 Smart Insights

**Smart Insights** is the AI-powered analysis engine behind My Metrics. It uses **machine learning** to automatically examine your data and surface meaningful patterns without requiring manual investigation.

### What Smart Insights Does

| Capability | Description |
|-----------|-------------|
| **Pattern Detection** | Automatically identifies hidden trends and anomalies in your data |
| **Automated Analysis** | Analyzes a selected data point without any manual effort |
| **Faster Decisions** | Reduces time spent on manual data exploration |
| **Contextual Observations** | Surfaces important observations relevant to your specific metric |

### How to Use Smart Insights

1. Select any **metric card** in My Metrics
2. Toggle **Smart Insights on** in the visualization area, **or**
3. Click the **Smart Insights option** directly from the card's action menu

> ⚠️ **Current Limitations:**
> - **Table widgets** are not yet supported
> - **Geo Map widgets** are not yet supported
> - Planned future enhancements include **scheduled metrics reports** and **recurrence pattern tracking**

---

## 13. 💡 Quick Summary

Here is an end-to-end overview of how everything connects in SAP Analytics Cloud:

```
🔐 Login
    │
    ▼
🏠 Home Screen
    ├── Today (pinned cards)
    ├── Catalog (published content)
    ├── Favorites
    └── Shared With Me
    │
    ▼
🧭 Navigate via Shell Bar & Side Navigation
    │
    ├── 👤 Profile & Settings
    │       ├── Profile picture
    │       ├── Language & Region
    │       └── Home Screen customization
    │
    ├── 📁 Files
    │       ├── My Files (root)
    │       ├── Public Folder
    │       ├── Samples
    │       └── Input Forms
    │
    ├── 🔗 Share Content
    │       ├── View / Edit / Full Control / Custom
    │       ├── Email notifications
    │       ├── Unshare anytime
    │       └── Schedule Publications (automated)
    │
    ├── 🌐 Content Network
    │       └── Transfer content between tenants
    │
    └── 📊 My Metrics
            ├── Your Metrics (cards)
            ├── Detailed Visualization (charts)
            └── Smart Insights (AI analysis)
```

---

## 📎 Additional Resources

| Resource | Link |
|----------|------|
| SAP Help Portal — Navigation | [Navigate in SAP Analytics Cloud](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) |
| SAP Help Portal — My Metrics | [Learn About My Metrics](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) |
| SAP Community Blog | [Introducing My Metrics](https://community.sap.com) |
| SAP Analytics Cloud Admin Course | Managing Security and Administration in SAP Analytics Cloud |

---

## 🏷️ Tags

`SAP` `SAP-Analytics-Cloud` `SAC` `Business-Intelligence` `Navigation` `File-Management` `My-Metrics` `Smart-Insights` `KPI` `Dashboard` `Data-Analytics`

---

> 📝 **Notes:** These study notes are based on SAP Analytics Cloud official learning content. SAP Analytics Cloud follows a **quarterly release cycle** — features and UI may vary slightly between versions.