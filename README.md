# AI-Powered Lead Qualification Engine

> An AI-driven Revenue Operations (RevOps) workflow that automatically captures, qualifies, scores, updates, and routes inbound leads using Make.com, HubSpot CRM, Google Gemini AI, and Gmail.

---

# Overview

This project automates one of the biggest challenges inside B2B sales teams:

> **How do we qualify inbound leads instantly without manual review?**

Instead of relying on SDRs or sales representatives to manually review every lead, this workflow evaluates each submission using AI, updates CRM records, and routes qualified opportunities automatically.

The entire process takes less than one minute and ensures that sales teams spend their time only on high-quality opportunities.

---

# Business Problem

Most B2B companies receive leads from website forms, landing pages, webinars, referrals, and campaigns.

Unfortunately, every lead is treated almost equally.

This creates several operational problems:

- Sales representatives waste time reviewing poor-quality leads.
- High-intent prospects wait too long for follow-up.
- CRM records remain incomplete.
- Lead qualification varies between team members.
- Marketing generates leads but Sales receives no quality assessment.
- Revenue teams lose opportunities because of delayed responses.

This results in lower conversion rates and revenue leakage.

---

# Solution

This automation creates an AI-powered qualification layer between Marketing and Sales.

Instead of manually reviewing every submission, the workflow:

✔ Captures new leads automatically

✔ Creates or updates the CRM record

✔ Sends lead information to Google Gemini AI

✔ AI evaluates ICP fit

✔ AI calculates qualification

✔ AI generates buying authority

✔ AI explains reasoning

✔ Updates HubSpot automatically

✔ Routes Qualified leads

✔ Sends instant notification email

The result is a standardized qualification process that improves speed, consistency, and CRM quality.

---

# Workflow Architecture

```
Tally Form
      │
      ▼
HubSpot CRM
(Create / Update Contact)
      │
      ▼
Google Gemini AI
(Lead Qualification)
      │
      ▼
HubSpot CRM
(Update AI Properties)
      │
      ▼
Router
 ┌───────────────┐
 │               │
 ▼               ▼
Qualified      Not Qualified
 │               │
 ▼               ▼
Gmail        Update Contact
```

---

# Workflow Screenshot
<img width="1231" height="577" alt="Lead Qualification Engine" src="https://github.com/user-attachments/assets/1fa34e09-083d-4a7e-9ae0-cc0294176b72" />

---

# Tech Stack

## Automation

- Make.com

## CRM

- HubSpot CRM

## AI

- Google Gemini AI

## Lead Capture

- Tally Forms

## Communication

- Gmail

## Logic

- Router
- Conditional Filters
- Structured AI Prompting

---

# Revenue Operations Layer

This project supports the following RevOps functions:

✅ Marketing Operations

- Lead Capture

- Form Automation

---

✅ Sales Operations

- Contact Creation

- CRM Synchronization

- AI Qualification

---

✅ Revenue Operations

- Lead Scoring

- Qualification Standardization

- CRM Hygiene

- Faster Lead Response

---

# Business Logic

Traditional Process

```
Lead Submitted

↓

Sales reviews manually

↓

Sales decides quality

↓

Updates CRM

↓

Follow-up
```

Problems

- Slow

- Subjective

- Manual

- Inconsistent

---

Pipeline Brain Process

```
Lead Submitted

↓

CRM Created

↓

AI Qualification

↓

Qualification Status

↓

CRM Updated

↓

Auto Routing

↓

Sales Notification
```

Benefits

- Consistent qualification

- Instant CRM updates

- Faster response

- Better SQL quality

- Reduced manual work

---

# Automation Steps

## Step 1

Trigger

Tally watches new submissions.

---

## Step 2

HubSpot

Create or update contact using email.

Mapped fields

- First Name

- Last Name

- Email

- Company

- Job Title

---

## Step 3

Google Gemini AI

Prompt receives

- Company

- Job Title

- Company Size

- Email

AI returns

- ICP Match Score

- Qualification Status

- Buying Authority

- Executive Reasoning

---

## Step 4

HubSpot Update

Update custom properties

- AI ICP Score

- Qualification

- Authority

- AI Notes

---

## Step 5

Router

Decision Engine

Route A

Qualified Lead

↓

Send Gmail notification

Route B

Not Qualified

↓

Update Contact Status

---

# AI Prompt

The workflow uses structured prompting with JSON responses to guarantee machine-readable outputs.

Expected JSON

```json
{
  "icp_match_score": 84,
  "qualification_status": "Qualified",
  "buying_authority": "Decision Maker",
  "reasoning_statement": "Manufacturing company with 500+ employees and senior purchasing authority."
}
```

---

# Screenshots

<img width="959" height="582" alt="Lead Qualification Engine 3" src="https://github.com/user-attachments/assets/7642add0-c59c-4105-9b43-c1972c314fbf" />
<img width="522" height="498" alt="Lead Qualification Engine 4" src="https://github.com/user-attachments/assets/abe0aad6-4180-412c-970a-4e76ab73249a" />
<img width="490" height="492" alt="Lead Qualification Engine 5" src="https://github.com/user-attachments/assets/7f4f7140-af2a-457a-b54f-6265be6ec01e" />
<img width="802" height="579" alt="Lead Qualification Engine 6" src="https://github.com/user-attachments/assets/05d9053b-484b-4306-9388-1f660460a96d" />
<img width="1086" height="578" alt="Lead Qualification Engine 2" src="https://github.com/user-attachments/assets/bf72a5f3-002e-4697-a8d4-cec73e9726d9" />

# Challenges Solved

## Challenge 1

Manual qualification

Solution

AI qualification

---

## Challenge 2

CRM inconsistency

Solution

Automatic HubSpot updates

---

## Challenge 3

Slow response

Solution

Instant routing

---

## Challenge 4

Different qualification standards

Solution

Single AI decision model

---

# Business Impact

Estimated Benefits

✔ Up to 70% reduction in manual lead qualification

✔ Faster lead response

✔ Improved CRM hygiene

✔ Better sales prioritization

✔ Higher SQL quality

✔ Consistent qualification framework

---

# RevOps Components Demonstrated

- Marketing Operations

- Lead Operations

- CRM Operations

- AI Qualification

- Workflow Automation

- Revenue Process Standardization

---

# Future Improvements

Version 2

- Apollo Enrichment

- AI Lead Scoring Engine

- Territory Routing

- Slack Notifications

- Revenue Leakage Detection

- Executive Dashboard

- Pipeline Forecasting

- Customer Success Integration

---

# Learning Outcomes

Through this project I learned:

- Make.com workflow architecture

- HubSpot CRM integration

- AI prompt engineering

- JSON-based structured AI responses

- CRM data synchronization

- Router and conditional logic

- Revenue Operations fundamentals

- Workflow documentation

---

# Next Project

➡️ OmniEngine: Enterprise Lead Orchestrator & Scoring Pipeline

This project expands the Lead Qualification Engine into a multi-source lead orchestration platform with Apollo enrichment, intelligent routing, database logging, and enterprise-grade RevOps automation.
