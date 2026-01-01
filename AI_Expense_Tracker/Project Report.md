# 📄 PROJECT SUBMISSION REPORT

## 1️⃣ Problem Chosen

> **“I earn good money, but every month I feel broke. Where is my money going?”**

---

## 2️⃣ Who the User Is

* Working professionals or students
* Comfortable using messaging apps
* Not disciplined enough to manually track expenses
* Wants clarity, not complex budgeting tools

---

## 3️⃣ When the Problem Feels Worst

* End of the month
* When savings are unexpectedly low
* When expenses feel invisible and untracked

---

## 4️⃣ What Users Have Already Tried

* Spreadsheet tracking (abandoned quickly)
* Expense apps (too many steps)
* Mental accounting (fails every time)

---

## 5️⃣ Why This Is Frustrating

Because the problem isn’t *earning* money —
it’s the **lack of awareness and feedback**.

---

## 6️⃣ Feature Built (Single Feature Focus)

### ✨ Feature: *Conversational Expense Logging*

**What it does**

* Lets users log expenses using natural language
* Automatically updates balance
* Warns users when balance gets low

**What it does NOT do**

* Budget forecasting
* Analytics dashboards
* Bank integrations


---

## 7️⃣ Why This Feature Was Chosen

* Extremely low friction
* Immediate value after one use
* Solves a single painful moment clearly

---

## 8️⃣ What Surprised Me While Building

* How effective natural language is for financial inputs
* How powerful simple automation can be without a full UI
* How much friction traditional apps introduce unnecessarily

---

## 9️⃣ Assumption I’m Least Certain About

That users will consistently use Telegram for financial tracking —
though early feedback suggests **chat-based logging feels natural**.

---

## 🔟 Would I Personally Use This?

Yes.
Because it requires **zero behavioral change**.


## 🏗️ Architecture Diagram

### Version 1 — Telegram Bot (Shipped ✅)

```
User (Telegram)
      |
      v
Telegram Bot Trigger
      |
      v
AI Agent (LLM + Business Logic)
      |
      +--> Memory (Context)
      |
      +--> Google Sheets (Ledger)
      |
      +--> Gmail (Low Balance Alert)
      |
      v
Telegram Response (Updated Balance)
```



## 1️⃣1️⃣ How This Could Become a Paid Product

* Multi-user accounts
* Monthly summaries
* Custom alert thresholds
* Multiple ledgers (personal + business)

---

## 1️⃣2️⃣ Future Development Scope (Version 2)

### 🚧 Planned but Not Implemented Yet

A **production-ready web application** version is planned using:

* **Lovable (frontend UI builder)**
* **n8n as backend automation engine**
* Google OAuth for user accounts
* Per-user Google Sheets

This version would support:

* Web-based input
* Multi-user dashboards
* Async webhook processing

### Version 2 — Production Web App (Planned 🚧)

```
Web App (Lovable UI)
        |
        v
API Gateway / Webhooks
        |
        v
n8n Backend Automation
        |
        +--> AI Agent (Intent Parsing)
        +--> Google Sheets / DB
        +--> Email Alerts
        |
        v
Async Response to UI
```

Preview:
![Image](https://github.com/Disha-Gupta-892/Workflow_Automations/blob/74af3173a53759dc537818b5f30155da25af6649/AI_Expense_Tracker/ExpenseFlow_Landscape_UI.png)

### ⚠️ Current Limitation

This version was **not implemented within the assignment window** due to:

* Insufficient API key limits
* OAuth and platform authentication constraints

However, the system design and backend automation logic are already validated in Version 1 and can be directly extended.

---

## 🏁 Final Reflection

This project demonstrates:

* Clear problem selection
* Strong scope control
* Real, usable output
* Builder-first mindset under time pressure

It prioritizes **working software over ideas**, exactly as required.

---
