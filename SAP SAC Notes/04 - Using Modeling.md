# 📊 SAP Analytics Cloud — Modeling Options, Models, Datasets & Data Sources

> Comprehensive reference guide on **Dimensions, Measures, Models (Analytic vs Planning), Datasets**, Live vs Import data, and creating basic models in SAP Analytics Cloud (SAC).

---

## 📚 Table of Contents

1. [Modeling Options Overview](#1--modeling-options-overview)
2. [Dimensions & Measures](#2--dimensions--measures)
3. [Models in SAP Analytics Cloud](#3--models-in-sap-analytics-cloud)
4. [Analytic vs Planning Models](#4--analytic-vs-planning-models)
5. [The Modeler](#5--the-modeler)
6. [Datasets in SAC](#6--datasets-in-sac)
7. [Datasets vs Models — Comparison](#7--datasets-vs-models--comparison)
8. [Model Data Sources: Live vs Import](#8--model-data-sources-live-vs-import)
9. [Modeling Workflow](#9--modeling-workflow)
10. [Creating a Live Model](#10--creating-a-live-model)
11. [Quick Summary](#11--quick-summary)

---

## 1. 📋 Modeling Options Overview

After completing this topic, you will be able to **differentiate between dimensions, models, and datasets**.

In SAP Analytics Cloud, data is organized using three core concepts:

- **Dimensions**
- **Models** (Analytic or Planning)
- **Datasets** (Embedded or Public)

These building blocks determine how you analyze, plan, and govern your data.

---

## 2. 📏 Dimensions & Measures

### Dimensions
**Dimensions** represent **categories** that provide context to numeric data.

**Examples**: Product Category, Date, Region, Customer, Cost Center.

- Can include **properties** (e.g., Customer Phone, Address)
- Support **hierarchies** (Year → Quarter → Month, Country → Region → City)

### Measures
**Measures** are the **numeric values** you analyze.

**Examples**: Sales Revenue, Quantity Sold, Salary, Gross Margin.

---

## 3. 🧩 Models

**Models** combine dimensions + measures and represent a specific business area (Sales, Finance, Production, etc.).

Models are the **primary data source** for stories in SAC.

---

## 4. ⚖️ Analytic vs Planning Models

| Model Type       | Access      | Key Features |
|------------------|-------------|--------------|
| **Analytic**     | Read-only   | Date optional, used for reporting & analysis |
| **Planning**     | Read/Write  | Includes Date + Version dimensions, supports budgeting & forecasting |

---

## 5. 🛠️ The Modeler

Central area in SAC to create and manage models.

**Creation Options**:
- Create a new model (Import)
- Create a Live Data Model

---

## 6. 📦 Datasets

Simple tabular data collections used for stories.

**Two Types**:
- **Embedded Dataset** → Inside one story only
- **Public Dataset** → Shareable across multiple stories

---

## 7. 🔍 Datasets vs Models — Comparison

| Aspect               | Datasets                     | Models                          |
|----------------------|------------------------------|---------------------------------|
| Use Case             | Ad-hoc, quick analysis       | Governed analysis & planning    |
| Planning             | Not supported                | Fully supported                 |
| Governance           | Low                          | High                            |
| Live Data Support    | Limited                      | Broad (SAP sources)             |

---

## 8. 🌐 Model Data Sources: Live vs Import

**Live Data** — Real-time, no data copied, SAP sources only.  
**Import Data** — Data copied into SAC, supports scheduling, works with SAP + Non-SAP.

---

## 9. 🔄 Modeling Workflow

1. Identify data sources
2. Choose Live or Import
3. Create Connection
4. Build Model (or Dataset)
5. Create Stories

---

## 11. 💡 Quick Summary

Here is an end-to-end overview of how everything connects in SAP Analytics Cloud modeling:
🔗 Data Sources
│
├── SAP Systems (HANA, BW, S/4HANA, Datasphere)
└── Non-SAP Sources (SQL, CSV, Google Drive, OData, etc.)
│
▼
🔌 Connections
├── Live Connection → Real-time, no data stored in SAC
└── Import Connection → Data copied + scheduled refresh
│
▼
🛠️ Modeler
├── Live Data Model (Analytic only)
└── Imported Model
├── Analytic Model (Read-only)
└── Planning Model (Read/Write + Version)
│
▼
📦 Data Objects
├── Models (Dimensions + Measures + Hierarchies)
└── Datasets
├── Embedded Dataset (story-specific)
└── Public Dataset (shareable)
│
▼
📊 Stories & Analysis
├── Visualizations
├── Planning Input
├── Data Analyzer
└── Insights