# 🤖 MeetSync AI – Meeting Summary & Follow-Up Agent

MeetSync AI is a fully autonomous agent that:
- 📝 Analyzes meeting transcripts
- 🧠 Summarizes key discussion points
- ✅ Extracts personalized to-do lists for each participant
- 📧 Sends the results via email
- 📅 Adds tasks directly to Google Calendar

> 🔗 Built using **n8n**, **LangChain**, and **Azure OpenAI (GPT-4o)**  
> 🛠️ Designed for the Mindcraft Hackathon 2025

---

## 🚀 Features

- ✅ One-click automation from transcript to tasks
- ✅ GPT-4o powered summarization & task extraction
- ✅ Instant email delivery of action items
- ✅ Automatic Google Calendar event creation
- ✅ 100% no-code/low-code implementation with n8n

---

## 🧠 How It Works

### 🌐 Workflow Overview

Webhook → Edit Fields (Transcript)
→ Basic LLM Chain (LangChain)
→ Extract Summary (Set Node)
→ Send Email (SMTP)
→ Create Google Calendar Event


---

### 📥 Sample Input

Alice: Please finish the report by Friday.
Bob: I’ll collect the data tomorrow.
Carol: I’ll handle the slides.


---

### 🤖 GPT Output

Summary: The team discussed tasks related to an upcoming report.

To-Do List:

Alice: Finish the report
Bob: Collect data
Carol: Prepare slides

---

## 🛠️ Tech Stack

| Tool           | Purpose                             |
|----------------|-------------------------------------|
| n8n            | Workflow automation platform        |
| LangChain      | LLM chain execution in n8n          |
| Azure OpenAI   | GPT-4o for summarization & tasks    |
| SMTP Email     | Sends summary via Gmail             |
| Google Calendar| Adds action items as calendar events|

---

## 📦 Files Included

- `MeetSync_Workflow.json` – Importable n8n workflow
- `README.md` – This file 😄
- `PPT_Presentation.pptx` – Project slides for submission (attached separately)

---

## ✅ How to Use

1. Clone or fork this repo
2. Open [n8n](https://n8n.io) (self-hosted or cloud)
3. Import `MeetSync_Workflow.json`
4. Update your:
   - SMTP credentials (Gmail recommended)
   - Azure OpenAI API key, deployment name
   - Google Calendar OAuth credentials
5. Trigger the webhook and see the automation in action!

---

## 💡 Future Enhancements

- Auto-import Google Meet transcripts
- Slack integration for real-time reminders
- Sentiment analysis of meeting tone
- Dashboard for tracking team progress

---

## 📧 Contact

Made by Aryan Mishra  
Submitted for the Mindcraft Hackathon 2025 🚀
