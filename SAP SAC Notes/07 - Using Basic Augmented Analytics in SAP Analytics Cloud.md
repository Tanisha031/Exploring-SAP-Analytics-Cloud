# 🤖 SAP Analytics Cloud — Augmented Analytics & AI-Powered Features

> A detailed reference guide covering SAP Analytics Cloud's AI and machine learning capabilities including Smart Insights, Smart Predict, and the Just Ask natural language query feature.

---

## 📚 Table of Contents

1. [What is Augmented Analytics?](#1--what-is-augmented-analytics)
2. [AI & ML Features Overview](#2--ai--ml-features-overview)
3. [Smart Predict](#3--smart-predict)
4. [Smart Insights](#4--smart-insights)
5. [Just Ask Feature](#5--just-ask-feature)
6. [Just Ask — User Interface Breakdown](#6--just-ask--user-interface-breakdown)
7. [Just Ask — Interaction Options](#7--just-ask--interaction-options)
8. [Joule Analytic Insights](#8--joule-analytic-insights)
9. [Hands-On Practice Scenario](#9--hands-on-practice-scenario)
10. [Quick Summary](#10--quick-summary)

---

## 1. 🧠 What is Augmented Analytics?

**Augmented Analytics** refers to the use of **Artificial Intelligence (AI)** and **Machine Learning (ML)** to automate data preparation, insight generation, and data analysis — making it easier for all users (not just data scientists) to understand their data and make decisions.

In SAP Analytics Cloud, augmented analytics features are built directly into the platform, meaning you don't need to be a data expert to benefit from them. The AI does the heavy lifting for you.

### Core Goal

> Take users from **raw data → actionable insights** faster, with less manual effort, using AI-powered automation.

---

## 2. 🗂️ AI & ML Features Overview

SAP Analytics Cloud provides the following AI and machine learning utilities:

| Feature | What It Does | Best For |
|---------|-------------|---------|
| **Smart Insights** | Automatically provides statistical insights about a data point or variance | Understanding *why* a number looks the way it does |
| **Smart Predict** | Learns from historical data to predict future events, values, and trends | Forecasting and predictive modeling |
| **Just Ask** | Natural language query (NLQ) interface — ask questions in plain language | Quick ad-hoc data exploration without building a story |
| **Compass Simulation** | Estimates possible outcomes of uncertain business events using Monte Carlo simulation | Scenario planning and risk analysis |
| **Joule Analytic Insights** | Conversational AI experience to explore SAC data from other SAP products | AI-driven exploration via chat interface |

---

## 3. 🔮 Smart Predict

**Smart Predict** enables users to build **predictive models** that automatically learn from historical data and generate predictions for the future — without requiring deep data science expertise.

### What Smart Predict Does

- Creates one or more **predictive scenarios** — preconfigured workspaces for building predictive models
- Automatically finds the **best relationships and patterns** in your historical data
- Generates **predictions** for future events, values, and trends
- Takes into account **trends, cycles, and fluctuations** in your data (especially in time series)

### Types of Predictive Scenarios

| Scenario Type | Description | Use Case Example |
|--------------|-------------|-----------------|
| **Classification** | Predicts which category/class a record belongs to | Will this customer churn? (Yes/No) |
| **Regression** | Predicts a numeric value based on input variables | What will next month's revenue be? |
| **Time Series** | Forecasts future values based on historical time-based data | Predict sales for the next 6 months |

### Supported Data Sources for Smart Predict

| Data Type | Supported? | Notes |
|-----------|-----------|-------|
| **Acquired data — Datasets** | ✅ Yes | Fully supported |
| **Acquired data — Planning Models** | ✅ Yes | Fully supported |
| **Acquired data — Analytic Models** | ❌ No | Not supported |
| **Live data — SAP HANA on-premise** | ✅ Yes | Only live source supported |
| **Other live connections** | ❌ No | Not supported |

> 📖 Smart Predict is covered in more detail in the **Applying AI-powered Visualizations and Augmented Analytics to Business Data in SAP Analytics Cloud** course.

---

## 4. 📊 Smart Insights

**Smart Insights** uses **statistical analysis** to automatically generate textual and visual explanations about your data — helping you understand *what* is happening and *why*.

### What Smart Insights Provides

- **Textual insights** — written explanations of key patterns and drivers
- **Visualizations** — charts that support the textual explanation
- Insights about a **specific data point** or a **variance** between values

### Where Smart Insights is Available

| Location | Available? |
|----------|-----------|
| **My Metrics** | ✅ Yes — via the Smart Insights panel |
| **Charts in Stories** | ✅ Yes — most chart types supported |
| **Table cells in Stories** | ✅ Yes |
| **All variance types in Stories** | ✅ Yes |

### Supported Data Sources for Smart Insights

| Data Source | Supported? |
|-------------|-----------|
| **Acquired data** | ✅ Yes |
| **Live SAP HANA connections** | ✅ Yes |
| **SAP Datasphere models** | ✅ Yes |
| **Seamless planning models** | ✅ Yes |

### How to Access Smart Insights

```
Option 1: My Metrics
    → Select a metric card
    → Smart Insights panel opens automatically on the right

Option 2: Story Chart
    → Right-click on a chart or table cell
    → Select "Smart Insights"
    → Insights panel opens with statistical analysis
```

> 📖 For more details, visit **Smart Insights on the SAP Help Portal**.

---

## 5. 💬 Just Ask Feature

The **Just Ask** feature is SAP Analytics Cloud's **Natural Language Query (NLQ)** interface. It allows you to ask questions about your data in **plain, everyday language** — and instantly receive results displayed as charts or tables.

> 💡 No need to build a story or know where the data lives. Just type your question and get an answer.

### Key Characteristics

| Property | Detail |
|----------|--------|
| **Input Method** | Natural language text query |
| **Supported Languages** | 🇬🇧 English · 🇩🇪 German · 🇫🇷 French · 🇮🇹 Italian · 🇪🇸 Spanish |
| **Output Formats** | Charts or simple tables |
| **Access Points** | Home screen · Shell bar icon |
| **Technology** | AI-driven Natural Language Query (NLQ) |

### Example Questions You Can Ask

```
"Show me sales by region"
"What were sales for 2023?"
"Sales for this quarter"
"Top 3 products by gross margin"
"Show me operating expenses by department"
"What is the revenue trend for the last 12 months?"
```

---

## 6. 🖥️ Just Ask — User Interface Breakdown

Here is a breakdown of the Just Ask interface and its key elements:

```
┌──────────────────────────────────────────────────────────────────┐
│  JUST ASK INTERFACE                                              │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│  [Select Model ▼]        [+ Add Model to Search]                │
│                                                                  │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  [+ Add to Search]   Type your question here...   [🔍]  │    │
│  └─────────────────────────────────────────────────────────┘    │
│                                                                  │
│  Keyword Suggestions: [ Sales ] [ Region ] [ Q1 ] [ Revenue ]   │
│                                                                  │
├──────────────────────────────────────────────────────────────────┤
│  RESULTS AREA                                                    │
│                                                                  │
│  [📊 Chart View]  [📋 Table View]  [🔍 Analyze]  [📋 Copy]  [⋮] │
│                                                                  │
│  ┌──────────────────────────────────────────────────────┐       │
│  │                                                      │       │
│  │              Chart / Table Result                    │       │
│  │                                                      │       │
│  └──────────────────────────────────────────────────────┘       │
│                                                                  │
│  💡 Suggestions: Related queries to explore further             │
│  📖 Prompt Guide: Tips & tricks for better queries              │
└──────────────────────────────────────────────────────────────────┘
```

### UI Elements Explained

| Element | Description |
|---------|-------------|
| **Select Model dropdown** | Choose which SAC model to query against |
| **Add Model to Search** | Add additional models to the current session |
| **+ Add to Search icon** | Browse available measures and dimensions to add to your query |
| **Search Field** | Type your natural language question here |
| **Auto-complete suggestions** | Appear as you type to help complete your query |
| **Keyword Suggestions** | System-generated keywords displayed below the search field; click to add to query |
| **Results Area** | Displays the chart or table result of your query |
| **Suggestions Section** | System-generated related queries to help explore the current data model further |
| **Prompt Guide** | Tips and tricks for writing better Just Ask queries |

### Model Indexing

> ⚠️ If a model you want to search is **not listed** in the dropdown:
> - Select **"Click here to create a model request to an admin"**
> - This sends a request for the model to be **indexed** for the Just Ask feature

---

## 7. ⚡ Just Ask — Interaction Options

After receiving results from a Just Ask query, you have several **interaction options** to further work with the data:

### Result Toolbar (Left to Right)

| Icon | Action | Description |
|------|--------|-------------|
| 📊 | **Chart View** | Display results as a chart visualization |
| 📋 | **Table View** | Switch to a tabular data display |
| 🔍 | **Analyze Data** | Opens **Data Analyzer** in a separate tab with the query results pre-loaded |
| 📋 | **Copy** | Copies the chart card to clipboard — paste into a story page using `Ctrl + V` |
| ⋮ | **More Options** | Additional options (see below) |

### More Options Menu

| Option | Description |
|--------|-------------|
| **Set Drill Level** | Set the starting drill level for the displayed data |
| **Reset Drill Level** | Reset the drill level back to default |
| **Sort Ascending** | Sort the displayed data from lowest to highest |
| **Sort Descending** | Sort the displayed data from highest to lowest |
| **Set Rank** | Apply a ranking (e.g., Top 5, Bottom 10) to the results |
| **Export as CSV** | Download the data as a CSV file |
| **Export as Excel** | Download the data as an Excel (.xlsx) file |

### How to Add a Just Ask Chart to a Story

```
Step 1: Run your query in Just Ask
Step 2: Click the Copy icon in the results toolbar
Step 3: Navigate to your story page
Step 4: Press Ctrl + V to paste the chart into the story
```

> 💡 This is a quick way to build stories from natural language queries without starting from scratch.

---

## 8. 🤝 Joule Analytic Insights

**Joule Analytic Insights** is the conversational AI experience that connects **SAP's AI copilot (Joule)** with SAP Analytics Cloud data.

### Key Points

| Property | Detail |
|----------|--------|
| **Where Joule Lives** | In **other SAP products** (not directly inside SAP Analytics Cloud) |
| **What It Does** | Allows users to explore SAC data via a conversational chat interface |
| **How It Works** | Powered by SAP Analytics Cloud's analytical engine in the background |
| **Availability** | Must be **enabled** in the SAP products you use |

### Joule vs Just Ask

| Feature | Just Ask | Joule Analytic Insights |
|---------|---------|------------------------|
| **Where to access** | Inside SAP Analytics Cloud | From other SAP products (e.g., S/4HANA) |
| **Interface type** | Search bar / NLQ | Conversational chat |
| **Output** | Charts and tables in SAC | Insights surfaced within the SAP product |
| **Primary user** | SAC users | Business users in SAP apps |

---

## 9. 🧪 Hands-On Practice Scenario

### Business Scenario

> You are working in a team responsible for reporting on **operating expenses** for your company. You're not sure where to start, so you decide to use the **Just Ask** feature in SAP Analytics Cloud to explore the data quickly.

### Task Flow

| Step | Task | What You Do |
|------|------|-------------|
| **Step 1** | Create a search query | Open Just Ask, select a model, and type a question about operating expenses |
| **Step 2** | Refine the query | Use keyword suggestions, auto-complete, or modify your question to drill deeper |
| **Step 3** | Add charts to a story | Copy the generated charts and paste them into a new or existing SAC story |

### Example Queries to Try

```
"Show operating expenses by department"
"Top 5 cost categories by total spend"
"Operating expenses for Q1 vs Q2 this year"
"Which department has the highest operating expenses?"
"Operating expense trend for the last 12 months"
```

---

## 10. 💡 Quick Summary

Here's how all the augmented analytics features fit together in SAP Analytics Cloud:

```
🤖 AUGMENTED ANALYTICS IN SAP ANALYTICS CLOUD
│
├── 🔮 Smart Predict
│       ├── Learn from historical data
│       ├── Predictive Scenarios: Classification · Regression · Time Series
│       └── Supported: Acquired datasets, planning models, SAP HANA live
│
├── 📊 Smart Insights
│       ├── Automatic statistical analysis
│       ├── Textual + visual explanations
│       ├── Available in: My Metrics · Charts · Tables · Variances
│       └── Supported: Acquired data · SAP HANA · Datasphere · Planning models
│
├── 💬 Just Ask (NLQ)
│       ├── Ask questions in plain language (EN, DE, FR, IT, ES)
│       ├── Get instant charts or tables
│       ├── Add results directly to stories (Copy → Ctrl+V)
│       ├── Open in Data Analyzer for deeper analysis
│       └── Export results as CSV or Excel
│
├── 🧭 Compass Simulation
│       └── Monte Carlo simulation for uncertain business scenario modeling
│
└── 🤝 Joule Analytic Insights
        ├── Conversational AI powered by SAC
        └── Accessed from other SAP products (not inside SAC directly)
```

### Feature Comparison at a Glance

| Feature | Skill Level Needed | Real-time? | Output |
|---------|-------------------|-----------|--------|
| **Smart Insights** | Beginner | ✅ Yes | Text + Chart explanations |
| **Smart Predict** | Intermediate | ❌ No (model training) | Predictive model + forecast |
| **Just Ask** | Beginner | ✅ Yes | Charts / Tables |
| **Compass** | Advanced | ❌ No | Simulation scenarios |
| **Joule** | Beginner | ✅ Yes | Conversational insights |

---

## 📎 Additional Resources

| Resource | Description |
|----------|-------------|
| [SAP Help Portal — Smart Insights](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Full documentation on Smart Insights |
| [SAP Help Portal — Smart Predict](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Full documentation on Smart Predict |
| [SAP Help Portal — Just Ask](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Natural language query documentation |
| [SAP Help Portal — AI-Assisted Calculations](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | AI formula generation documentation |
| SAP Course | Applying AI-powered Visualizations and Augmented Analytics to Business Data in SAP Analytics Cloud |

---

## 🏷️ Tags

`SAP` `SAP-Analytics-Cloud` `SAC` `Augmented-Analytics` `AI` `Machine-Learning` `Smart-Insights` `Smart-Predict` `Just-Ask` `NLQ` `Natural-Language-Query` `Joule` `Predictive-Analytics` `Business-Intelligence`

---

> 📝 **Notes:** These study notes are based on SAP Analytics Cloud official learning content. AI and ML features may require administrator enablement before use. Always check feature availability for your specific SAP Analytics Cloud version and license.