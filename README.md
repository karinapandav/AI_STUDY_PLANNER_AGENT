# AI Study Planner Agent

An AI-powered study planner that generates personalized study schedules using **Google Gemini**, automatically stores them in **Google Sheets**, and schedules study sessions in **Google Calendar** through **n8n** workflows.

---

## 🚀 Features

- 🤖 AI-powered personalized study plan generation
- 🧠 Google Gemini integration
- 💬 Conversational AI Agent with memory
- 📋 Structured JSON output using Output Parser
- 📊 Automatic logging to Google Sheets
- 📅 Automatic Google Calendar event creation
- 🔄 Split study plans into individual tasks
- ⚡ End-to-end workflow automation with n8n

---

## 🛠️ Tech Stack

- n8n
- Google Gemini
- Google Sheets API
- Google Calendar API
- AI Agent
- Structured Output Parser
- Simple Memory

---

## 📂 Workflow Overview

```
Chat Trigger
      │
      ▼
AI Agent
      │
      ▼
Google Gemini
      │
      ▼
Structured Output Parser
      │
      ▼
Split Out
     ├────────► Google Sheets
     └────────► Google Calendar
```

---

## 📌 Current Status

### ✅ Milestone 1 – AI Study Planner MVP
- Chat-based AI study planner
- Google Gemini integration
- Structured JSON output
- Google Sheets integration

### ✅ Milestone 2 – Google Calendar Integration
- Automatic creation of study sessions in Google Calendar
- Personalized scheduling based on AI-generated study plans

---

## 🚧 Upcoming Features

- Intelligent conflict detection
- Adaptive study plan rescheduling
- Email reminders
- Telegram / WhatsApp notifications
- Weekly progress reports
- Study analytics dashboard
- PDF study plan export
- Deployment and live demo

---

## 📁 Repository Structure

```
ai-study-planner-agent/
│
├── README.md
├── workflows/
│   └── ai-study-planner.json
└── screenshots
```

---

## 👨‍💻 Author

**Karina Pandav**
