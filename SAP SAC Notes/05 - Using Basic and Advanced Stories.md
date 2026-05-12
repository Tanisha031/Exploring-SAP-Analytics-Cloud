# 📖 SAP Analytics Cloud — Viewing, Interacting & Building Stories

> Complete guide on how to view, interact with, personalize, export, and build stories in SAP Analytics Cloud (SAC).

---

## 📚 Table of Contents
1. [Introduction to Stories](#1-introduction-to-stories)
2. [Working Modes](#2-working-modes)
3. [Bookmarks in Stories](#3-bookmarks-in-stories)
4. [Exporting Stories & Data](#4-exporting-stories--data)
5. [More Options & More Actions](#5-more-options--more-actions)
6. [Building Simple Stories](#6-building-simple-stories)
7. [Story Design Elements](#7-story-design-elements)
8. [Microsoft Office Add-ins Integration](#8-microsoft-office-add-ins-integration)
9. [Advanced Scripted Stories](#9-advanced-scripted-stories)
10. [Quick Summary](#10-quick-summary)

---

## 1. Introduction to Stories

An **SAP Analytics Cloud Story** is the main medium for **data reporting, visualization, and analysis**. It can function as a dashboard, detailed report, or interactive analysis tool containing charts, tables, filters, and more.

Stories usually contain multiple **pages** — some for high-level summaries (dashboards) and others for detailed analysis.

---

## 2. Working Modes

Every story in SAC supports **three working modes**:

### View Mode
- Default mode when opening a story.
- Read-only experience.
- You can interact with filters, input controls, drill-downs, and hover tooltips, but **cannot modify** the story design.

### Edit Mode
- Full design control.
- Add, rearrange, format, and configure widgets, pages, and interactivity.
- Used by content designers and analysts.

### Present Mode
- Turns your story into an interactive, fluid presentation.
- Retains full interactivity and real-time data.
- Ideal for meetings and fact-based decision making.
- No separate license required.

---

## 3. Bookmarks in Stories

**Bookmarks** let you save specific views (filters, prompts, selections) of a story for quick access later.

### Why Use Bookmarks?
- Avoid resetting filters every time
- Switch between different scenarios instantly
- Share exact views with colleagues

### Key Features
- Can be **Private** (personal) or **Global/Public**
- You need appropriate permissions to create global bookmarks
- Can be set as the **default view** for a story
- Supports **Customize Link** for meaningful URLs
- Bookmarks can be shared

---

## 4. Exporting Stories & Data

### Export Entire Story
From **File → Export**, you can export the full story as:
- **PDF**
- **PowerPoint (PPTX)**
- **Google Slides**

> Note: This exports a static snapshot (not interactive, data not refreshed automatically).

### Export Data from Widgets
- Use the **More Actions** button (⋯) on any chart or table
- Export underlying data as **CSV** or **Excel (XLSX)**

---

## 5. More Options & More Actions

### More Options (...)
- Appears in various places depending on screen size and zoom level.
- Provides additional settings and commands.

### More Actions (⋯)
- Available on **every widget** (charts, tables, images, text, etc.)
- Acts like a right-click context menu
- Options differ between **View** and **Edit** mode
- Includes **Export Data** option for charts and tables

---

## 6. Building Simple Stories

### Starting a New Story
You can:
- Start with a **Blank Page**, or
- Use a **Pre-built Template** (SAP or company-specific)

### Page Types
- **Responsive** → Automatically adjusts for different screen sizes (recommended for mobile)
- **Canvas** → Fixed layout

### Adding Widgets
- Use the top **Story Toolbar** (Chart, Table, etc.)
- Or drag & drop from the **Left Side Panel (Assets)**

---

## 7. Story Design Elements

### Toolbar & Panels
- **Story Toolbar**: File, Edit, Insert, Tools, Format, View
- **Left Side Panel**:
  - **Assets** → Widgets & elements
  - **Outline** → Pages & scripting
  - **Filters** → Story-level filters
- **Right Side Panel**:
  - **Builder** → Add dimensions/measures
  - **Styling** → Formatting options

### Data Sources
When adding a widget, select:
- A **Model** (recommended)
- A **Dataset**
- Live connection to SAP Datasphere or other sources

### Design Guidelines
- Keep it simple
- Define clear visual hierarchy
- Group related information together
- Follow natural reading direction

---

## 8. Microsoft Office Add-ins Integration

### SAP Analytics Cloud Add-in for Microsoft Excel
- Bring SAC data directly into Excel
- Supports hierarchies, formulas (`SAP.GETDATA`), planning (write-back, publish)
- Real-time analysis and formatting

### SAP Analysis for Microsoft Office
- Powerful multidimensional analysis tool
- Works with SAC live connections
- Includes Analysis + EPM plug-ins

### SAP Analytics Cloud Add-in for Microsoft PowerPoint
- Embed live SAC widgets into slides
- Refresh data directly in PowerPoint
- Includes **AI-assisted chart summary** (generative AI)

---

## 9. Advanced Scripted Stories

For highly customized experiences, you can add **scripting** to stories.

- Uses a **subset of JavaScript**
- Enables advanced interactivity and custom behaviors
- Can restrict or enhance standard functionality
- Script Editor includes auto-complete, syntax check, and Ctrl+Space suggestions

> Usually developed in collaboration with IT/developers.

---

## 10. Quick Summary

| Feature                  | View Mode | Edit Mode | Present Mode |
|-------------------------|-----------|-----------|--------------|
| Interactivity           | Yes       | Yes       | Yes          |
| Design & Edit           | No        | Yes       | No           |
| Export Story            | Yes       | Yes       | -            |
| Export Widget Data      | Yes       | Yes       | -            |
| Bookmarks               | Yes       | Yes       | -            |
| Scripting               | -         | Yes       | -            |

**Best Practices**:
- Use **Responsive** pages for broad access
- Create **Bookmarks** for common views
- Leverage **Microsoft Add-ins** for Office users
- Export data via **More Actions** for analysis outside SAC

---

**Made with ❤️ for the SAP Community**  
*Last Updated: May 2026*

---

## 🔗 Related Guides
- [Core Concepts: Measures & Dimensions](../core-concepts.md)
- [Models & Datasets](../modeling.md)
- [Planning in SAC](../planning.md)
