# 🧠 n8n Todoist Task Snooze Workflow

This automation does the following:
- Moves tasks from `Inbox` to `Snoozed` project if their due date is in future.
- Brings them back to `Inbox` 3 days before due date.

## 🔧 Setup Instructions

1. Add your Todoist credentials in n8n.
2. Create a Todoist project named `snoozed`.
3. Update the project IDs in the workflow nodes:
   - `Set inbox project id` – set to your Inbox project ID.
   - `Set snoozed project id` – set to your `snoozed` project ID.
4. Activate the workflow.

## 📂 File

- `todoist-snooze-workflow.json`: Full n8n workflow.

## 👨‍💼 Author

- Email: kbhargav924@gmail.com
- GitHub: [bhargav2601-art](https://github.com/bhargav2601-art)
- LinkedIn: [Bhargav K](https://www.linkedin.com/in/bhargav-k-bab841296)