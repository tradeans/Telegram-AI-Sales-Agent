# 🤖 AI Sales Bot with Human-in-the-Loop Governance

> **A production-grade Telegram bot that automates sales, manages inventory, and escalates to humans when needed.**  
> Built with **n8n**, **Airtable**, **OpenAI**, and **Slack**.

---

## 🎥 Demo
[![Watch the Demo](https://drive.google.com/file/d/1pv3jkjl67ItTWmULAOEisZxGOuYYowza/view?usp=drive_link)
> *Click to watch the 3-minute walkthrough of the bot in action.*

---

## 🚀 Business Value
| Feature | Impact |
| :--- | :--- |
| **24/7 Automated Sales** | AI handles inquiries, stock checks, and orders instantly. |
| **Zero Overselling** | Real-time stock deduction ensures inventory accuracy. |
| **Human Oversight** | Admins approve orders via interactive buttons, preventing fraud. |
| **Seamless Escalation** | Customers can request human help; admins get instant alerts. |
| **Proactive Ops** | Low stock alerts and fulfillment tracking keep operations smooth. |
| **Production Reliability** | Centralized error logging and Slack alerts ensure uptime. |

---

## 🏗️ Architecture
![System Architecture]

*   **Telegram:** Customer and admin interface with interactive UI.
*   **n8n:** Workflow orchestration, AI agent logic, and integrations.
*   **Airtable:** Database for products, orders, sessions, and error logs.
*   **OpenAI:** LLM with tool calling, memory, and guardrails.
*   **Slack:** Dedicated channel for critical error alerts.

---

## ✨ Key Features
### 🛒 AI-Powered Sales
- Natural language product lookup with accurate stock/pricing.
- Order creation with validation and currency enforcement (₱).
- Conversation memory for contextual interactions.

### 👤 Human-in-the-Loop
- **Order Approval:** Admins receive order details with Approve/Reject buttons.
- **Stock Deduction:** Inventory updates only after approval.
- **Handoff Escalation:** AI detects handoff requests, alerts admin, and pauses until reset.

### 📦 Operational Excellence
- **Low Stock Alerts:** Proactive notifications when inventory drops below threshold.
- **Order Fulfillment:** Customers receive shipment updates with tracking numbers.
- **Error Handling:** All errors logged to Airtable; critical issues alert Slack.

---

## 🛠️ Tech Stack
- **Automation:** n8n (Workflow Orchestration)
- **AI:** OpenAI GPT-4 (Tool Calling, Memory)
- **Database:** Airtable (Relational Data, Audit Logs)
- **Frontend:** Telegram Bot API (Interactive UI)
- **Observability:** Slack (Alerts), Airtable (Logs)
- **Language:** JavaScript (Code Nodes, Expressions)

---

## 📂 Workflows
- [`ai-sales-bot.json`](./workflows/ai-sales-bot.json) - Main AI agent with tools and memory.
- [`order-approval.json`](./workflows/order-approval.json) - Approval flow with stock deduction.
- [`human-handoff.json`](./workflows/human-handoff.json) - Escalation and reset mechanism.
- [`low-stock-alerts.json`](./workflows/low-stock-alerts.json) - Proactive inventory monitoring.
- [`order-fulfilled.json`](./workflows/order-fulfilled.json) - Shipment notifications.
- [`global-error-handler.json`](./workflows/global-error-handler.json) - Centralized error logging.

---

## 🚀 Setup
See [SETUP.md](./docs/SETUP.md) for detailed installation instructions.

---

## 👤 Author
**Kevyn Alojepan**  
AI Automation Engineer | n8n Expert  
📧 [your-email@example.com]  
🔗 [LinkedIn Profile]  
🌐 [Portfolio Website]
