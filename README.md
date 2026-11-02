# 💱 Automated Multi-Currency FX Rate Alert Automation

An automated foreign exchange (FX) monitoring and notification pipeline built with **n8n**. The workflow automatically fetches daily exchange rates for major global currencies against the Nigerian Naira (NGN), formats structured rate bulletins, and publishes instant updates to a designated Telegram channel.

---

## 🚀 Key Features

- **Automated Daily Trigger:** Scheduled cron execution to fetch market exchange rates at set daily intervals.
- **Multi-Currency Tracking:** Fetches and processes rates for **USD, GBP, EUR, CAD, and KWD** relative to **NGN**.
- **API Data Fetching:** Integrates with financial exchange rate APIs using n8n HTTP Request nodes.
- **Data Transformation & Formatting:** Uses custom JavaScript expressions to format currency values, compute rate variations, and structure clean Markdown messages.
- **Telegram Broadcast Integration:** Dispatches structured bulletins directly to a Telegram group/channel via the Telegram Bot API.

---

## 🛠️ Tech Stack & Tools

- **Workflow Automation:** [n8n](https://n8n.io/)
- **API Integration:** HTTP Request Node / Financial FX API
- **Messaging Service:** Telegram Bot API
- **Data Manipulation:** JavaScript / Node.js runtime inside n8n

---

## 🛠️ Setup & Installation

### 1. Requirements
- Self-hosted or Cloud **n8n** instance.
- **Telegram Bot Token** (created via [@BotFather](https://t.me/BotFather)).
- Active **Telegram Chat ID** / Channel handle.
- Financial FX API Key (if required by your endpoint).

### 2. Import Workflow
1. Download `fx_rate_alert_workflow.json` from this repository.
2. In your n8n workspace, navigate to **Workflows** $\rightarrow$ **Import from File**.
3. Select `fx_rate_alert_workflow.json`.

### 3. Credential Configuration
- Add your **Telegram API** credential in the Telegram node.
- Configure your API endpoint and authentication (if applicable) in the HTTP Request node.

---

## 💡 Use Case & Value

Navigating currency fluctuations requires timely, hands-off market awareness. This pipeline eliminates manual checking by delivering structured, real-time rate bulletins directly to mobile and desktop devices via Telegram, ensuring quick insights for financial monitoring and conversion decisions.

---

## 👤 Author

**Clinton Agummadu (Odogwu)**
* AI Automation Specialist & Workflow Engineer
* **GitHub:** [@Clinton-Agummadu](https://github.com/Clinton-Agummadu)
* **LinkedIn:** [Clinton Agummadu](www.linkedin.com/in/clinton-agummadu-602389288)
