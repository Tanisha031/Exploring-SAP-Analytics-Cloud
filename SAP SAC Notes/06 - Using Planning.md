# 📊 SAP Analytics Cloud — Planning Features & Manual Planning

> Comprehensive guide to **Planning Capabilities** in SAP Analytics Cloud (SAC) — including data entry, versions, data actions, value driver trees, Compass simulations, and more.

---

## 📚 Table of Contents
1. [Introduction to Planning](#1-introduction-to-planning)
2. [Planning Features Overview](#2-planning-features-overview)
3. [Data Entry](#3-data-entry)
4. [Version Management](#4-version-management)
5. [Data Locking](#5-data-locking)
6. [Data Actions](#6-data-actions)
7. [Validation Rules](#7-validation-rules)
8. [Value Driver Trees](#8-value-driver-trees)
9. [Structured Allocations](#9-structured-allocations)
10. [SAP Analytics Cloud Compass Simulations](#10-sap-analytics-cloud-compass-simulations)
11. [Manual Input Planning Tasks](#11-manual-input-planning-tasks)
12. [Quick Summary](#12-quick-summary)

---

## 1. Introduction to Planning

**Planning** in SAP Analytics Cloud is a collaborative process for setting strategic goals, creating budgets, generating forecasts, and simulating scenarios.

It combines historical **Actuals** data with future projections, departmental input, market trends, risks, and opportunities.

SAC provides a complete **enterprise planning** solution integrated with analytics — allowing you to plan, analyze, and act in one unified platform.

> **Note**: Basic data entry is available with a BI license. Full planning features (publishing versions, advanced tools) require a **Planning License**.

---

## 2. Planning Features Overview

SAC offers powerful planning tools:

- Data Entry
- Version Management
- Data Locking
- Data Actions
- Validation Rules
- Value Driver Trees
- Structured Allocations
- Compass Simulations

These features support both **structured** and **ad-hoc** planning workflows.

---

## 3. Data Entry

- Performed directly in **tables** inside stories
- Supports **absolute** and **relative** values (`*2`, `+500`, etc.)
- Copy cell values with aggregation logic
- Plan at any hierarchy level — values automatically disaggregate
- Unsaved changes appear in **yellow**
- Supports **undo/redo** before publishing

---

## 4. Version Management

Versions allow you to work with multiple scenarios safely:

- Compare **Actuals** vs **Budget** vs **Forecast**
- Create **Private Versions** for personal work
- Publish versions when ready
- Variance analysis
- History tracking and rollback
- Work on scenarios without affecting original data

---

## 5. Data Locking

- Lock specific sections of data during closing periods
- Delegate locking rights to data owners
- Set data to **Restricted** mode (only owners can edit)
- Schedule locking changes via the **Calendar**

---

## 6. Data Actions

Data Actions let you automate planning sequences using a visual (no-code) interface.

### Available Steps:
- Copy Step
- Cross-Model Copy
- Allocation Step
- Conversion Step
- Fact Deletion
- Advanced Formulas Step
- Embedded Data Action

**Use Cases**: Cash flow planning, depreciation, carry-forward, copying data between models, etc.

- Supports **parameters** for flexibility
- Can be run manually in stories or **scheduled** via Calendar
- AI-assisted script generation available (if enabled)

---

## 7. Validation Rules

- Define valid **member combinations** across dimensions
- Prevents invalid data entry
- Example: Allow planning only for specific Product + Location combinations

---

## 8. Value Driver Trees

Visual driver-based planning tool for simulations and strategic decisions.

- Built directly in stories
- Automatically creates nodes from Account structure
- Visualize value flow and impact on KPIs
- Great for scenario modeling and "what-if" discussions

---

## 9. Structured Allocations

- Reusable allocation logic (e.g., IT costs by headcount, travel costs by region)
- Built with visual tools inside Data Actions
- Supports complex allocation rules without coding

---

## 10. SAP Analytics Cloud Compass Simulations

**Compass** is a native Monte Carlo simulation engine for analyzing uncertainty.

### Compass vs Time Series Forecasting

| Feature                        | Compass Simulation          | Time Series Forecast       |
|--------------------------------|-----------------------------|----------------------------|
| Needs Historical Data          | No                          | Yes                        |
| Needs Defined Driver Relations | Yes                         | No                         |
| Method                         | Monte Carlo (probabilities) | Trend projection           |
| Best For                       | "What if things change?"    | "What if trend continues?" |

**Use Cases**: Risk assessment, target setting, budget reviews, strategic planning.

---

## 11. Manual Input Planning Tasks

Typical workflow includes:
- Creating a planning story with configured tables
- Using simulation features
- Working with private versions
- Publishing approved data
- Applying data locks

---

## 12. Quick Summary

| Feature                | Purpose                              | License Needed     |
|------------------------|--------------------------------------|--------------------|
| Data Entry             | Manual input & calculations          | BI + Planning      |
| Version Management     | Scenarios & private work             | Planning           |
| Data Locking           | Control editing during close         | Planning           |
| Data Actions           | Automation & complex logic           | Planning           |
| Value Driver Trees     | Driver-based simulations             | Planning           |
| Compass                | Uncertainty & risk simulation        | Planning           |

**Key Benefits of SAC Planning**:
- Real-time collaboration
- Integrated analytics + planning
- No-code advanced features
- Strong Microsoft Office integration
- AI assistance

---

**Made with ❤️ for the SAP Analytics Community**  
*Last Updated: May 2026*

---

## 🔗 Related Guides
- [Stories & Visualization](../stories-guide.md)
- [Models & Dimensions](../modeling-guide.md)
- [Navigation & Home Screen](../navigation-guide.md)

---

**Tags**:  
`SAP` `SAP-Analytics-Cloud` `SAC` `Planning` `Budgeting` `Forecasting` `Data-Actions` `Value-Driver-Trees` `Compass` `Monte-Carlo`