# Gmail Coupon Summary with n8n

This project uses [n8n](https://n8n.io) to automate the extraction of coupon codes from promotional Gmail emails and sends a daily summary email with the extracted information.

## 🔧 Workflow Description

- **Trigger**: Runs daily (e.g., cron or manual trigger)
- **Step 1**: Fetch Gmail messages from the "Promotions" label
- **Step 2**: Extract coupon codes, discount percentages, and expiry dates
- **Step 3**: Trash processed emails
- **Step 4**: Generate and send a styled summary email

## 📂 Files

- `promosweep.json`: Exported n8n workflow

## 💡 Tech Stack

- **n8n** for automation
- **Gmail API** for email access
- **Custom JavaScript** in n8n's Function nodes
- **HTML/CSS** for summary email design

## 🖼 Example Output

![Summary Email Example](screenshots/summary-email.png)

## 🧪 Run Locally

You can import the JSON file into a self-hosted or cloud n8n instance. The logic for extracting coupons still needs some improvement. 

## 🔐 Security

OAuth2 is used to connect to Gmail. No credentials are stored in this repo.

---

