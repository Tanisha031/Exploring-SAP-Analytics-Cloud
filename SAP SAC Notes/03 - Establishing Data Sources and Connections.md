# 🔌 SAP Analytics Cloud — Data Sources, Connections & Data Analyzer

> A detailed reference guide covering SAP Analytics Cloud connection types, data sources, and how to create insights using the Data Analyzer tool.


---

## 📚 Table of Contents

1. [What is a Connection?](#1--what-is-a-connection)
2. [Types of Connections](#2--types-of-connections)
3. [Live vs Import — Detailed Comparison](#3--live-vs-import--detailed-comparison)
4. [Choosing the Right Connection](#4--choosing-the-right-connection)
5. [Data Analyzer Overview](#5--data-analyzer-overview)
6. [Data Analyzer User Interface](#6--data-analyzer-user-interface)
7. [Key Features of Data Analyzer](#7--key-features-of-data-analyzer)
8. [Saving an Insight](#8--saving-an-insight)
9. [AI-Assisted Calculations in Data Analyzer](#9--ai-assisted-calculations-in-data-analyzer)
10. [Hands-On Practice Scenario](#10--hands-on-practice-scenario)
11. [Quick Summary](#11--quick-summary)

---

## 1. 🔌 What is a Connection?

A **Connection** in SAP Analytics Cloud is the communication bridge between SAP Analytics Cloud and an external **data source**. Without a connection, SAC cannot access or display any data.

### Key Rules About Connections

- Every connection is tied to **one specific data source**
- If your organization uses **multiple data sources**, you need **multiple connections**
- Connections can point to both **cloud-based** and **on-premise** data sources
- Connections are typically set up by **system administrators**

```
┌─────────────────────┐          ┌──────────────────────────┐
│                     │          │                          │
│  SAP Analytics      │◄────────►│   Data Source            │
│  Cloud (SAC)        │          │   (SAP HANA, BW,         │
│                     │  Connection  Google Drive, SQL, etc.)│
└─────────────────────┘          └──────────────────────────┘
```

> 💡 One Connection = One Data Source. Multiple sources require multiple connections.

---

## 2. 🔄 Types of Connections

SAP Analytics Cloud supports **two types** of connections:

| Connection Type | Description |
|----------------|-------------|
| **Live Connection** | Queries data directly from the source in real-time — no data is imported into SAC |
| **Import Connection** | Copies/imports data into SAC's internal storage for offline analysis |

---

## 3. 📊 Live vs Import — Detailed Comparison

### Live Connection

```
SAP Analytics Cloud  ◄──── Real-time query ────►  SAP Data Source
     (no data stored)                              (SAP BW, SAP HANA, etc.)
```

| Property | Details |
|----------|---------|
| **Data Storage** | No data stored in SAC — data stays in the source system |
| **Data Freshness** | Always real-time and up-to-date |
| **Supported Sources** | **SAP systems only** (e.g., SAP BW, SAP HANA, SAP S/4HANA) |
| **Best For** | Scenarios requiring real-time data accuracy |
| **Limitations** | Cannot connect to non-SAP sources |

### Import Connection

```
SAP Analytics Cloud  ◄──── Data copied/imported ────  Any Data Source
   (data stored in SAC)                               (SAP or Non-SAP)
```

| Property | Details |
|----------|---------|
| **Data Storage** | Data is **imported and stored** inside SAC |
| **Data Freshness** | Depends on refresh schedule — may not be real-time |
| **Supported Sources** | SAP **and** Non-SAP sources |
| **Non-SAP Examples** | Google Drive · SQL Databases · OData Services · REST APIs · CSV Files |
| **Best For** | Scenarios with large data volumes or non-SAP sources |
| **Limitations** | Data can become stale without regular refreshes |

### Side-by-Side Comparison

| Criteria | Live Connection | Import Connection |
|----------|----------------|-------------------|
| **Real-time data** | ✅ Yes | ❌ No (scheduled refresh) |
| **SAP sources** | ✅ Yes | ✅ Yes |
| **Non-SAP sources** | ❌ No | ✅ Yes |
| **Data stored in SAC** | ❌ No | ✅ Yes |
| **Data privacy risk** | 🔒 Lower (data stays at source) | ⚠️ Higher (data copied to SAC) |
| **Large data volumes** | ⚠️ May affect performance | ✅ Better for large volumes |
| **Internet dependency** | ✅ Requires constant connection | ❌ Works offline after import |

---

## 4. ✅ Choosing the Right Connection

Your organization must evaluate which connection type best fits your **unique needs**. Consider the following criteria when making this decision:

### Evaluation Criteria

#### 1. 📋 Functional Needs
- Do you need **real-time data** for decision-making? → Use **Live**
- Do you need to connect to **non-SAP systems** like Google Drive or SQL? → Use **Import**
- Do you need **offline access** to data? → Use **Import**

#### 2. 🔒 Data Privacy Constraints
- Does your organization have policies against **copying sensitive data** outside its original system? → Use **Live**
- Are there **regulatory requirements** about where data can be stored? → Review carefully before using **Import**

#### 3. 📦 Data Volume Constraints
- Do you work with **very large datasets** that may impact query performance? → Use **Import** (pre-aggregated)
- Is your data **relatively small** and manageable in real-time? → **Live** works well

### Decision Flowchart

```
Is your data source an SAP system?
         │
    ┌────┴────┐
   YES        NO
    │          │
    ▼          ▼
Do you need    Use IMPORT Connection
real-time      (non-SAP sources only
data?          supported here)
    │
 ┌──┴──┐
YES    NO
 │      │
 ▼      ▼
Use    Use IMPORT
LIVE   Connection
```

> ⚠️ **Important:** Always review the **SAP Analytics Cloud System Requirements and Technical Prerequisites** in the SAP Help Portal to ensure your landscape is compliant with the supported versions and connection types.

---

## 5. 🔍 Data Analyzer Overview

**Data Analyzer** is a **predefined, ready-to-run application** inside SAP Analytics Cloud designed for **ad-hoc analysis** — meaning you can explore and analyze data on the fly without building a full story first.

### Supported Data Sources in Data Analyzer

| Data Source | Type |
|-------------|------|
| **Live SAP BW Queries** | Live Connection |
| **Live SAP HANA Views** | Live Connection |
| **SAP Analytics Cloud Models** | Native SAC models |
| **SAP Datasphere Models** | Connected Datasphere models |

### Key Advantage

> 💡 All Live SAP BW queries, Live SAP HANA views, and models are accessible **directly** in the selection dialogs — **no additional model needs to be created** before you start your analysis.

### What You Can Do with Data Analyzer

- Perform **ad-hoc data exploration** without a predefined story
- **Drill down** into data details interactively
- **Save your drill-down state** as a reusable **Insight**
- Use it directly **within an SAP Analytics Cloud story** as an embedded component

---

## 6. 🖥️ Data Analyzer User Interface

The Data Analyzer interface is divided into several key areas:

```
┌────────────────────────────────────────────────────────────────┐
│  Menu Bar  [ Refresh ]  [ Edit Prompts ]  [ Save ]             │
├──────────────────────┬─────────────────────────────────────────┤
│                      │                                         │
│   Builder Panel      │         Data View                       │
│                      │   (Table View  OR  Chart View)          │
│  ┌────────────────┐  │                                         │
│  │   Dimensions   │  │   Rows and columns of data with         │
│  │   (drag & drop)│  │   applied dimensions and measures       │
│  ├────────────────┤  │                                         │
│  │   Measures     │  │                                         │
│  │   (drag & drop)│  │                                         │
│  └────────────────┘  │                                         │
├──────────────────────┴─────────────────────────────────────────┤
│  Filter Area — Apply filters to narrow down your data view     │
└────────────────────────────────────────────────────────────────┘
```

### UI Components Explained

| Component | Description |
|-----------|-------------|
| **Menu Bar** | Contains Refresh, Edit Prompts, and Save options |
| **Data View** | Displays data in either **tabular** (table) or **chart** format — switchable |
| **Filter Area** | Apply filters to focus on specific data segments |
| **Builder Panel** | Drag-and-drop panel to add/remove **dimensions** and **measures** from the analysis |
| **Edit Prompts Dialog** | Available when your data source uses prompts (variables); lets you set prompt values |
| **Refresh** | Re-queries the data source to get the latest data |

---

## 7. ⚙️ Key Features of Data Analyzer

### 📐 Tabular vs Chart View

| View | Best For |
|------|---------|
| **Tabular View** | Precise numbers, detailed row-level analysis, comparisons |
| **Chart View** | Visual trends, patterns, and high-level overviews |

> You can switch between both views at any time during your analysis.

### 🧮 Calculated Measures

- Create **custom calculations** directly within Data Analyzer
- These calculations **exist only within the insight** — they are NOT written back to the source data model
- Useful for quick one-off analysis without modifying the underlying model

### 🎨 Conditional Formatting

- Apply **visual formatting rules** to highlight specific data values
- Examples: color-code cells based on thresholds, highlight negative values in red, etc.
- Helps surface important data points at a glance

### 🔽 Drag-and-Drop Builder

- The **Builder Panel** allows intuitive drag-and-drop of dimensions and measures
- Add or remove fields from the analysis without writing any code
- Rearrange columns and rows interactively

### 🔁 Prompts (Variables)

- If your data source (e.g., SAP BW query) is designed with **prompts/variables**, the **Edit Prompts** dialog allows you to set values for those prompts before running the analysis
- This filters the data at the source level for better performance

---

## 8. 💾 Saving an Insight

After drilling down and analyzing your data to the desired level of detail, you can **save your work as an Insight** for future use.

### How to Save an Insight

1. Click **Save** in the **upper left corner** of the Data Analyzer
2. The **Save Insight** dialog appears
3. Select the **file location** where you want to save the insight
4. Enter a **name** for the insight
5. Enter an optional **description** for context
6. Click **Save**

> 📌 **What gets saved?**
> The saved insight preserves:
> - Your **drill-down state** (what dimensions/measures are displayed)
> - Applied **filters**
> - Any **calculated measures** you created
> - **Conditional formatting** rules

---

## 9. 🤖 AI-Assisted Calculations in Data Analyzer

SAP Analytics Cloud includes **AI-assisted calculation features** in the Data Analyzer that make building formulas faster and more accessible — especially for users who are not formula experts.

> ⚙️ **Prerequisite:** This feature must be **enabled by your administrator** before it becomes available.

### Two AI Capabilities

#### 1. 🪄 Generate (Natural Language → Formula)

- Type a **plain language description** of the calculation you want
- The AI **translates** your description into a valid SAC calculation formula
- Example: *"Show me the percentage difference between this year and last year sales"* → AI generates the formula automatically

#### 2. 💬 Explain (Formula → Natural Language)

- Select an **existing complex formula**
- The AI **explains the formula in plain, simple language**
- Helps business users understand what a formula does without needing technical knowledge

### AI Calculation Workflow

```
User types natural language query
            │
            ▼
    AI (Generate) processes the query
            │
            ▼
    Formula is generated in the calculation dialog
            │
            ▼
    User reviews and applies the formula
            │
            ▼
    Formula is used within the Insight (not saved to data source)
```

> 📖 For more details, visit the SAP Help Portal: **Using AI-Assisted Calculations**

---

## 10. 🧪 Hands-On Practice Scenario

### Business Scenario

> Your team has asked you to create a data insight that accesses data from **SAP HANA** — without performing a data import. You need to add formatting and a custom calculation to make the insight more useful.

### Task Flow

Follow these steps in the practice exercise:

| Step | Task | Details |
|------|------|---------|
| **Step 1** | Create a new insight | Select SAP HANA as the live data source in Data Analyzer |
| **Step 2** | Add Conditional Formatting | Apply color rules to highlight important values in the table |
| **Step 3** | Add a Calculated Measure | Create a custom formula-based measure within the insight |

### Why Use Live Connection Here?

- The scenario specifies **no data import** → This means a **Live Connection** to SAP HANA is required
- Data stays in SAP HANA; SAC queries it in real-time
- No model needs to be created beforehand — SAP HANA views are directly accessible in Data Analyzer

---

## 11. 💡 Quick Summary

Here is a full overview of how data sources, connections, and Data Analyzer work together:

```
📦 Data Sources
    ├── SAP Sources (BW, HANA, S/4HANA, Datasphere)
    └── Non-SAP Sources (Google Drive, SQL, OData, CSV, etc.)
            │
            ▼
🔌 Connections
    ├── LIVE Connection
    │       ├── SAP sources only
    │       ├── Real-time data
    │       └── No data stored in SAC
    │
    └── IMPORT Connection
            ├── SAP + Non-SAP sources
            ├── Data copied into SAC
            └── Needs scheduled refresh for updates
            │
            ▼
🔍 Data Analyzer
    ├── Ad-hoc analysis (no story needed)
    ├── Tabular or Chart view
    ├── Drag-and-drop Builder Panel
    ├── Filters + Prompts
    ├── Calculated Measures (insight-only)
    ├── Conditional Formatting
    └── AI-Assisted Calculations
            │   ├── Generate (text → formula)
            │   └── Explain (formula → text)
            │
            ▼
💾 Saved Insight
    └── Preserves drill-down state, filters, calculations, and formatting
```

---

## 📎 Additional Resources

| Resource | Description |
|----------|-------------|
| [SAP Help Portal — System Requirements](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Technical prerequisites and supported connection types |
| [SAP Help Portal — AI-Assisted Calculations](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Full documentation on using AI for formula generation |
| [SAP Help Portal — Data Analyzer](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Complete Data Analyzer feature reference |
| [SAP Help Portal — Connections](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Guide to creating and managing connections |

---

## 🏷️ Tags

`SAP` `SAP-Analytics-Cloud` `SAC` `Data-Sources` `Live-Connection` `Import-Connection` `Data-Analyzer` `SAP-HANA` `SAP-BW` `Ad-Hoc-Analysis` `AI-Assisted` `Business-Intelligence`

---

> 📝 **Notes:** These study notes are based on SAP Analytics Cloud official learning content. Always verify connection compatibility with your specific SAP Analytics Cloud version and system landscape before implementation.