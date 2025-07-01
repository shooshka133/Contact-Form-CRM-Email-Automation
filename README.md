# 📬 Contact Form CRM + Email Automation (n8n)

This project captures form submissions from a GitHub-hosted HTML form and automates syncing to Google Sheets, Airtable, and email delivery — all using n8n.

## 🌐 Live Form
Hosted on GitHub Pages using `index.html`.

## ⚙️ What It Does

- 📥 Captures form submissions via **Webhook**
- 📝 Formats data using **Set Node**
- 📄 Appends to **Google Sheets**
- 📋 Creates a new record in **Airtable**
- 📧 Sends a confirmation **Email** to the user

## 🧱 Workflow Structure

```
Webhook → Set Fields → [ Google Sheets | Airtable | Email ]
```

## 🛠 Tools Used

| Tool         | Purpose                         |
|--------------|----------------------------------|
| n8n          | Automation workflow              |
| Google Sheets| CRM entry storage                |
| Airtable     | Filtering & tagging              |
| Gmail (n8n)  | Auto-email to user               |
| GitHub Pages | Form hosting                     |

## 📝 Fields Tracked

- `name`
- `email`
- `message`
- `submitted_at` (auto timestamp)

## 📂 Files in This Repo

- `index.html` – The contact form (hosted)
- `Contact_Form_Workflow.json` – n8n export file
- `README.md` – This file
- `screenshots/` – Optional screenshots of workflow and results

## ✅ Setup Instructions

1. Import `Contact_Form_Workflow.json` into your n8n.
2. Replace the webhook URL in `index.html` with your n8n webhook.
3. Set up credentials for:
   - Google Sheets (OAuth2)
   - Airtable
   - Gmail
4. Deploy the form on GitHub Pages or similar.
5. Submit the form to see data flow into your CRM and inbox!

---

**Built with ❤️ using n8n**