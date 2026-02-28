# 🔁 n8n Automation Workflows – Todoist & Telegram Bot

Welcome to a collection of advanced automation workflows built using [n8n](https://n8n.io). These flows streamline productivity with task management and AI-powered news delivery.

---

## 📌 Included Workflows

### ✅ 1. Todoist Auto Snooze/Unsnooze Workflow

**Goal**: Automatically move tasks with due dates from your **Inbox** to a `Snoozed` project, and return them back **3 days before their due date**.

#### 🔄 How it works:
- Every **5 minutes**: Tasks with future due dates are snoozed (moved to `Snoozed`).
- Every day at **5 AM**: Tasks are unsnoozed and returned to `Inbox` 3 days before the due date.
- Skips subtasks and ensures project IDs don’t conflict.

#### 🛠 Setup:
1. Add your Todoist OAuth credentials in n8n.
2. Create a Todoist project called `Snoozed`.
3. Update the correct project IDs inside the workflow nodes:
   - **Inbox project ID**
   - **Snoozed project ID**
4. Import the `todoist-snooze-workflow.json` file into n8n and activate.

---

### 📲 2. Telegram AI News Bot – Country & Topic Aware

**Goal**: Let users ask for news on specific topics and countries in natural language, and get AI-filtered GNews headlines via Telegram.

#### 🧠 Smart Features:
- Understands messages like:
  - `tech news in japan`
  - `cricket india`
  - `gaza conflict`
- Extracts **topic** and **country** using a custom logic node.
- Uses the **GNews API** to fetch top 5 headlines.
- Formats and sends results directly back to the user on Telegram.

#### 🛠 Setup:
1. Create a Telegram bot using [@BotFather](https://t.me/BotFather).
2. Add the Telegram bot credentials in n8n.
3. Set up a **Webhook Trigger** node using your bot token.
4. Add your **GNews API key** to the HTTP Request node.
5. Import the `telegram-news-bot.json` into n8n and activate it.

---

## 🧾 File Overview

| File Name                     | Description                                |
|------------------------------|--------------------------------------------|
| `todoist-snooze-workflow.json` | Automates snoozing and unsnoozing tasks in Todoist |
| `telegram-news-bot.json`       | Telegram chatbot that responds with live news |
| `README.md`                    | Complete setup and documentation           |

---

## 👨‍💻 Author

- **Bhargav K**
- 📧 Email: [kbhargav924@gmail.com](mailto:kbhargav924@gmail.com)
- 🔗 LinkedIn: [linkedin.com/in/bhargav-k-bab841296](https://www.linkedin.com/in/bhargav-k-bab841296)
- 🐙 GitHub: [github.com/bhargav2601-art](https://github.com/bhargav2601-art)

---

> ⚡ These workflows were built to automate daily routines and boost productivity. Clone, customize, and deploy!