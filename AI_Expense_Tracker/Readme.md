# 🤖 AI-Powered Expense Tracker (Telegram Bot + n8n)

An end-to-end **AI-powered personal expense tracking system** that allows users to log expenses using **natural language messages** on Telegram.
The system automatically categorizes expenses, maintains a running balance, stores records in Google Sheets, and sends **low-balance alerts via email** — all without requiring a traditional app or manual data entry.

This project focuses on solving one real problem simply and effectively:

> **“I earn money, but I don’t know where it goes every month.”**

---

## 🚀 What This Automation Does

✔️ Accepts expense inputs via **Telegram chat**

✔️ Understands **free-text messages** like “Spent 500 on food”

✔️ Uses AI to extract:

* Credit / Debit
* Expense type
* Amount
* Updated balance

✔️ Automatically updates a **Google Sheet ledger**

✔️ Sends an **email alert** when balance falls below a threshold

✔️ Responds back to the user with updated balance in real time

In short:
**Message → AI Understanding → Ledger Update → Alert → Feedback**

---

## 🧠 High-Level Workflow Architecture (Version 1)

1. **Telegram Trigger**

   * Listens for incoming user messages
   * Acts as the primary user interface

2. **AI Agent (LLM-powered)**

   * Parses natural language expense input
   * Classifies transaction as credit or debit
   * Calculates updated balance
   * Applies business rules (low balance check)

3. **Memory Layer**

   * Maintains short conversational context
   * Enables follow-up interactions

4. **Google Sheets – Balance Updater**

   * Appends structured expense records
   * Acts as a lightweight persistent database

5. **Email Alert System**

   * Automatically triggers when balance ≤ threshold
   * Notifies user to prevent overspending

6. **Telegram Response**

   * Confirms transaction
   * Shows updated balance instantly

---

## 🧩 Tools & Technologies Used

| Category            | Tool / Platform  |
| ------------------- | ---------------- |
| Workflow Automation | n8n              |
| Messaging Interface | Telegram Bot API |
| AI Model            | OpenAI (LLM)     |
| Memory              | LangChain Memory |
| Data Storage        | Google Sheets    |
| Notifications       | Gmail API        |

---

## 🧪 Example User Inputs

* “Spent 250 on groceries”
* “Paid rent 8000”
* “Got salary 25000”
* “Coffee 150”

No predefined commands.
No rigid format.
Just natural language.

---

## 🔒 Reliability & Safety

* Read/write limited to user-owned Google Sheet
* No financial integrations (no bank access)
* Email alerts are informational only
* All logic is deterministic and auditable

---

## 📈 Why This Matters

Most expense apps fail because:

* They require too much manual effort
* They interrupt the user’s natural behavior

This system meets the user **where they already are** — chat — and removes friction entirely.

---

## 👤 Author

**Disha Gupta**

AI Automation Engineer

Focused on building **practical, AI-driven tools** that solve everyday problems with minimal user effort.

---
