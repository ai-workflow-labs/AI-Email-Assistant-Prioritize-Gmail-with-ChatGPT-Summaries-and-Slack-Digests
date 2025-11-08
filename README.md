<img width="637" height="201" alt="image" src="https://github.com/user-attachments/assets/27b7ecfd-1d49-46d3-b526-b27d6dd7a8ab" />
# 📬 Smart Email Prioritization & Slack Summary Workflow

Automate your inbox like a pro — never miss an important investor or lead email again.  
This lightweight workflow uses **Gmail**, **ChatGPT**, and **Slack** to classify, summarize, and organize emails automatically.  

---

## 💡 Use Cases

- 🧠 **Prevent missed investor or lead emails**  
- 🗂️ **Use Google Sheets as a lightweight CRM**  
- 🔔 **Get Slack summaries of critical Gmail activity**  
- 🕒 **Automate daily insights without manual checks**

---

## 🔧 How It Works

1. 📥 **Gmail Node** — Fetches new messages using Gmail API.  
2. 🤖 **ChatGPT Node** — Summarizes content, detects urgency & classifies email type (lead, investor, info, etc.).  
3. 🚨 **High/Medium Urgency** —  
   - Sent instantly to **Slack**  
   - Labeled in **Gmail** for quick visibility  
4. 📝 **Low Urgency** — Logged in **Google Sheets** for reference.  
5. ⏰ **Cron Node (Daily at 7 PM)** — Sends a concise **Slack summary** of the day’s Gmail activity.

---

## ✅ Requirements

| Tool | Purpose |
|------|----------|
| 🔑 **OpenAI API Key** | For GPT-4 or GPT-4o-based summarization & classification |
| 📧 **Gmail Access** | Read and label permissions |
| 💬 **Slack Bot Token / Webhook URL** | For message notifications and summaries |
| 📊 **Google Sheets Integration (optional)** | For CRM-style data logging |

---

## 🛠 Customization Ideas

- 💬 Replace **Slack** with **Telegram** or **WhatsApp** for instant updates  
- 🧾 Route **investor leads** to **Airtable** or **Notion** for advanced CRM workflows  
- 🌍 Add **multi-language support** via ChatGPT prompt customization  
- 📅 Create **weekly summaries** and send them via **email or Slack**

---

## ⚙️ Tech Stack

- 🧩 **n8n / Make / Zapier** (any automation platform)  
- 🤖 **OpenAI GPT-4 / GPT-4o**  
- 📧 **Gmail API**  
- 💬 **Slack API**  
- 📊 **Google Sheets API**  

---

## 🧠 Example Output

**Slack Message Example:**
> 🚨 *New Investor Email Detected!*  
> **From:** John Doe (VC Partner)  
> **Subject:** Follow-up on Investment Deck  
> **Urgency:** High  
> **Summary:** John is requesting your updated financial projections before Friday.  
> *(Labeled as “Investor Priority” in Gmail)*

---

## 🪄 Future Enhancements

- 🧱 AI-based sentiment and tone detection  
- 🕹️ Smart auto-responder for low-priority emails  
- 📈 Dashboard with lead statistics and summary analytics  
- 🌐 Integration with CRMs like HubSpot or Pipedrive

---

## 🚀 Quick Setup

1. Connect **Gmail**, **Slack**, and **OpenAI** nodes.  
2. Set **Cron** to run every day at `19:00` (7 PM).  
3. Paste your **API keys** in environment variables.  
4. Test the workflow → Watch your Slack light up with smart insights.  
