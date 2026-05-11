# Setup Instructions

## Prerequisites
- n8n account (Cloud or Self-Hosted)
- Airtable base with schema (Products, Orders, Chat_Sessions, Error_Logs)
- Telegram Bot Token
- OpenAI API Key
- Slack Bot Token (for error alerts)

## Installation
1. Import workflows from `/workflows` folder into n8n.
2. Configure credentials in n8n.
3. Update workflow variables (Admin Chat ID, Slack Channel ID).
4. Activate workflows.

## Airtable Schema
- **Products:** `name`, `stock`, `low_stock_threshold`, `low_stock_alert_sent`
- **Orders:** `order_id`, `status`, `quantity`, `tracking_number`, `fulfillment_notified`
- **Chat_Sessions:** `chat_id`, `human_mode`, `handoff_alert_sent`
- **Error_Logs:** `workflow_name`, `node_name`, `error_message`, `severity`, `resolved`
