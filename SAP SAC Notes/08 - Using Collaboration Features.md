# 💬 SAP Analytics Cloud — Discussions, Comments & Calendar

> A detailed reference guide covering SAP Analytics Cloud collaboration features including Discussions, Comments, AI-assisted commenting, and the Calendar task management system.

---

## 📚 Table of Contents

1. [Collaboration Overview](#1--collaboration-overview)
2. [Discussions Feature](#2--discussions-feature)
3. [Comments Feature](#3--comments-feature)
4. [Comment Rules & Limits](#4--comment-rules--limits)
5. [AI-Assisted Commenting](#5--ai-assisted-commenting)
6. [Discussions vs Comments — Comparison](#6--discussions-vs-comments--comparison)
7. [SAP Analytics Cloud Calendar](#7--sap-analytics-cloud-calendar)
8. [Calendar Tasks](#8--calendar-tasks)
9. [Scheduled Publications in Calendar](#9--scheduled-publications-in-calendar)
10. [Hands-On Practice Scenarios](#10--hands-on-practice-scenarios)
11. [Full Collaboration Flow Summary](#11--full-collaboration-flow-summary)

---

## 1. 🤝 Collaboration Overview

SAP Analytics Cloud provides two primary collaboration tools that allow teams to communicate, provide feedback, and manage work — all **within the platform** without switching to external tools.

| Tool | Purpose | Best For |
|------|---------|---------|
| **Discussions** | Team-based conversations and messaging | Ongoing team communication about a story or topic |
| **Comments** | Targeted feedback on specific story elements | Precise, data-point-level feedback and annotations |
| **Calendar** | Task creation, assignment, and tracking | Workflow management and scheduled publications |

---

## 2. 💬 Discussions Feature

The **Discussion** feature allows you to collaborate with team members in a chat-style conversation directly within SAP Analytics Cloud — without leaving the platform.

### How to Start a Discussion

```
Step 1: Select the Collaboration icon in the story or interface
Step 2: Choose one or more people to collaborate with
Step 3: Start your conversation
```

### What You Can Do in a Discussion

| Action | Description |
|--------|-------------|
| **Send Messages** | Write and send text messages to collaborators |
| **Add Attachments** | Attach files to provide additional context |
| **Link to Stories** | Use the **+ icon** at the bottom of the panel to link other stories |
| **Tag Users** | Mention team members directly to notify them |
| **Use in Calendar Tasks** | Discussions can also be used within calendar tasks for task-level collaboration |

### Where the Discussion Panel Appears

- In the **Collaboration panel** within stories
- In the **Calendar** task details
- Profile pictures and names of all participants are visible in the panel
- **Hover over a profile picture** to view the full user profile or start a **one-to-one private discussion**

---

## 3. 📝 Comments Feature

**Comments** allow you to leave targeted, specific feedback on individual elements within a story — going deeper than discussions by attaching feedback directly to **data points, widgets, or pages**.

### How to Add a Comment

```
Step 1: Select the element you want to comment on
        (a chart, table, data point, or story page)
Step 2: Click the Comment icon
Step 3: Type your message
Step 4: Tag team members using @ if needed
Step 5: Submit the comment
```

### Where You Can Comment

| Location | Description |
|----------|-------------|
| **Story Page** | Leave a general comment on an entire page of the story |
| **Data Point** | Comment directly on a specific value in a chart or table cell |
| **Widget** | Comment on a specific chart, table, or other widget element |

### Additional Comment Capabilities

- **Tag users** with `@username` to notify specific team members
- **Export comments** to a file directly from the story
- **SAP Analytics Cloud keeps a full commenting history** — all past comments are tracked and accessible

---

## 4. 📏 Comment Rules & Limits

| Rule | Detail |
|------|--------|
| **Standard comment limit** | Up to **10,000 characters** per comment |
| **Dimension comment limit** | Up to **255 characters** per comment |
| **Comment history** | SAC keeps track of the **full commenting history** |
| **Export** | Comments can be **exported to a file** from the story |

> ⚠️ Comments on **dimensions** have a significantly lower character limit (255 vs 10,000). Plan your feedback accordingly.

---

## 5. 🤖 AI-Assisted Commenting

SAP Analytics Cloud includes **AI-assisted commenting** features to make your collaboration smarter and more efficient.

> ⚙️ **Prerequisite:** This feature must be **enabled by your administrator** before it is available.

### What AI-Assisted Commenting Can Do

| Capability | Description |
|-----------|-------------|
| **Summarize Comments** | Automatically summarizes comments on **table data cells** or within a **comment widget** — extracting key information and insights |
| **Summarize Comment Threads** | Applies to both **individual comments** and **entire comment threads** |
| **Summarize Descendant Comments** | Within tables, summarize comments from **descendants of a parent node** |
| **Rephrase Text** | Before submitting a comment, AI can **rephrase your text** to make your message clearer and more effective |

### AI Comment Workflow

```
You write a comment draft
        │
        ▼
AI offers to rephrase it for clarity
        │
        ▼
You review and approve the rephrased version
        │
        ▼
Comment is posted on the data cell or widget
        │
        ▼
Later: AI can summarize the full comment thread
        │
        ▼
Key insights are extracted automatically
```

### Where AI-Assisted Commenting Works

- ✅ **Table data cells** — summarize and rephrase
- ✅ **Comment widgets** in stories — summarize and rephrase
- ✅ **Comment threads** — full thread summarization
- ✅ **Parent node descendants** in tables — summarize child-level comments

> 📖 For more details, visit the SAP Help Portal:
> - **Use AI-Assisted Commenting for Data Point Comments**
> - **Use AI-Assisted Features of Comment Widget in Stories**

---

## 6. ⚖️ Discussions vs Comments — Comparison

| Criteria | Discussions | Comments |
|----------|------------|---------|
| **Purpose** | Team-wide collaboration and messaging | Targeted feedback on specific elements |
| **Scope** | Broad — story level or general topic | Precise — data point, widget, or page level |
| **Attachments** | ✅ Yes | ❌ No |
| **Story Linking** | ✅ Yes (via + icon) | ❌ No |
| **@ Tagging** | ✅ Yes | ✅ Yes |
| **History Tracking** | ✅ Yes | ✅ Yes |
| **Export** | ❌ No | ✅ Yes (to file) |
| **AI Assistance** | ❌ No | ✅ Yes (summarize & rephrase) |
| **Character Limit** | No specific limit mentioned | 10,000 (255 for dimensions) |
| **Best For** | Ongoing team conversations | Precise, data-level annotations |

---

## 7. 📅 SAP Analytics Cloud Calendar

The **SAP Analytics Cloud Calendar** is a built-in task and workflow management tool that helps you **organize, assign, track, and review work** — all within SAP Analytics Cloud.

### What the Calendar Helps You Do

| Capability | Description |
|-----------|-------------|
| **Collaborate** | Work with colleagues on shared tasks |
| **Set & Track Statuses** | Monitor the progress of tasks (e.g., In Progress, Completed) |
| **Assign Reviewers** | Designate specific users to review completed work |
| **Add Reminders** | Set reminders so deadlines are never missed |
| **View Due Dates** | See all task deadlines in a calendar view |
| **Manage Scheduled Publications** | View and manage story scheduling jobs |

---

## 8. ✅ Calendar Tasks

### Types of Tasks

The calendar supports different types of tasks to match your workflow needs:

| Task Type | Description |
|-----------|-------------|
| **General Task** | A standard task that can be assigned to one or more users |
| **Composite Task** | A parent task that contains multiple sub-tasks managed together |

### Creating a Task — Key Steps

```
Step 1: Open the SAP Analytics Cloud Calendar
Step 2: Create a new task (General or Composite)
Step 3: Set the task name, description, and due date
Step 4: Assign the task to a team member
Step 5: Assign a Reviewer (someone who will review the completed work)
Step 6: Add reminders if needed
Step 7: Save the task
```

### Task Roles

| Role | Description |
|------|-------------|
| **Creator** | The person who creates the task |
| **Assignee** | The person responsible for completing the task |
| **Reviewer** | The person who reviews and approves the completed task |

### Task Status Tracking

Once a task is created, the status moves through stages:

```
Created → In Progress → Submitted for Review → Reviewed / Completed
```

### Using Discussions Within Tasks

- Each calendar task has a **built-in Discussion feature**
- Assignees, reviewers, and creators can communicate directly within the task
- Keeps all task-related communication **organized in one place**

---

## 9. 📆 Scheduled Publications in Calendar

The Calendar also serves as a management hub for **Scheduled Publications** — automated story distributions you have configured.

### What You Can Do with Scheduled Publications in the Calendar

| Action | Description |
|--------|-------------|
| **View** | See all active and upcoming scheduled publication jobs |
| **Modify** | Update the schedule, recipients, or frequency |
| **Copy** | Duplicate an existing schedule as a template |
| **Discontinue** | Pause or stop a schedule without deleting it |
| **Delete** | Permanently remove a scheduled publication |

> ⚠️ **Permission Note:** Users with the **Manage permission on Schedule Publication** can alter schedules **created by other users**.

---

## 10. 🧪 Hands-On Practice Scenarios

### Scenario 1 — Discussions & Comments

> **Business Context:** You are part of an international team analyzing a story. You need to communicate with team members about the story content using SAP Analytics Cloud's collaboration tools.

| Step | Task |
|------|------|
| **Step 1** | Add a comment on a **widget** in the story |
| **Step 2** | Add a comment on a **page** in the story |
| **Step 3** | Turn off **comment mode** when done |
| **Step 4** | Use the **Discussion feature** to provide feedback to the team |

---

### Scenario 2 — Calendar Collaboration

> **Business Context:** In a meeting, it was decided to update a story by removing dimensions from a table. A colleague has offered to complete the task. You use the Calendar to manage this collaboration.

| Step | Task | Details |
|------|------|---------|
| **Task 1** | Share the story | Share with **Full Control** access so the assignee can edit |
| **Task 2** | Create a General Task | Define a **reviewer** and set due dates and reminders |
| **Task 3** | Use Discussion in task | Communicate within the task using the Discussion feature |
| **Task 4** | Complete as Assignee | Log in as the assignee and complete the task |
| **Task 5** | Verify completion | View the calendar task to confirm it is marked as completed |

---

## 11. 💡 Full Collaboration Flow Summary

Here's how all collaboration tools work together in SAP Analytics Cloud:

```
👥 COLLABORATION IN SAP ANALYTICS CLOUD
│
├── 💬 DISCUSSIONS
│       ├── Start from the Collaboration icon
│       ├── Add team members
│       ├── Send messages, attachments, story links
│       └── Available in: Stories · Calendar Tasks
│
├── 📝 COMMENTS
│       ├── Comment on: Story Pages · Widgets · Data Points
│       ├── Tag users with @username
│       ├── Export comment history to file
│       ├── Limit: 10,000 chars (255 for dimensions)
│       └── 🤖 AI-Assisted Commenting (if enabled)
│               ├── Summarize comment threads
│               ├── Rephrase your text for clarity
│               └── Summarize parent node descendants (tables)
│
└── 📅 CALENDAR
        ├── Task Types: General · Composite
        ├── Roles: Creator · Assignee · Reviewer
        ├── Track: Status · Due Dates · Reminders
        ├── Discuss within tasks (built-in Discussion)
        └── 📆 Scheduled Publications Management
                ├── View · Modify · Copy
                └── Discontinue · Delete
```

### Feature Quick Reference

| Feature | Where to Access | Requires Admin Enable? |
|---------|----------------|----------------------|
| **Discussions** | Collaboration icon in story | ❌ No |
| **Comments** | Comment icon on element | ❌ No |
| **AI Comment Summary** | Comment panel (table/widget) | ✅ Yes |
| **AI Comment Rephrase** | Comment input field | ✅ Yes |
| **Calendar Tasks** | Calendar in side navigation | ❌ No |
| **Scheduled Publications** | Calendar view | ❌ No (requires Schedule privilege) |

---

## 📎 Additional Resources

| Resource | Description |
|----------|-------------|
| [SAP Help Portal — AI-Assisted Commenting (Data Points)](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Use AI-Assisted Commenting for Data Point Comments |
| [SAP Help Portal — AI Comment Widget](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Use AI-Assisted Features of Comment Widget in Stories |
| [SAP Help Portal — Calendar](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Full Calendar and task management documentation |
| [SAP Help Portal — Discussions](https://help.sap.com/docs/SAP_ANALYTICS_CLOUD) | Collaboration and discussion feature documentation |

---

## 🏷️ Tags

`SAP` `SAP-Analytics-Cloud` `SAC` `Collaboration` `Discussions` `Comments` `AI-Assisted` `Calendar` `Task-Management` `Scheduled-Publications` `Business-Intelligence` `Teamwork`

---

> 📝 **Notes:** This is the **final module** of the SAP Analytics Cloud study notes series. These notes are based on SAP Analytics Cloud official learning content. AI-assisted features require administrator enablement. Always verify feature availability for your specific SAP Analytics Cloud version and license tier.

---

## 📦 Full Study Notes Series

> All modules in this SAP Analytics Cloud GitHub study notes collection:

| # | Module | Topic |
|---|--------|-------|
| 1 | `SAP_BDC_and_Analytics_Cloud_Intro.md` | SAP Business Data Cloud & SAC Introduction |
| 2 | `SAP_Analytics_Cloud_Terminology.md` | Key Terminology |
| 3 | `SAP_Analytics_Cloud_Navigation_Files_Metrics.md` | Navigation, Files & My Metrics |
| 4 | `SAP_Analytics_Cloud_Data_Sources_Connections_DataAnalyzer.md` | Data Sources, Connections & Data Analyzer |
| 5 | `SAP_Analytics_Cloud_Augmented_Analytics_AI.md` | Augmented Analytics & AI Features |
| 6 | `SAP_Analytics_Cloud_Discussions_Comments_Calendar.md` | ⭐ Discussions, Comments & Calendar *(This File)* |