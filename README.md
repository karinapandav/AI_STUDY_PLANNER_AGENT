# 📚 AI Study Planner Agent

An AI-powered Study Planner built using **n8n**, **Google Gemini**, **Google Sheets**, and **Google Calendar**. The assistant generates personalized study schedules, automatically logs them to Google Sheets, schedules them in Google Calendar, and intelligently reschedules study sessions through natural language.

---

# 🚀 Features

- 🤖 AI-powered personalized study plan generation
- 🧠 Google Gemini integration
- 💬 Conversational AI Agent with memory
- 📋 Structured JSON output using Output Parser
- 📊 Automatic logging to Google Sheets
- 📅 Automatic Google Calendar event creation
- 🔄 AI-powered study plan rescheduling
- 🎯 Intent-based workflow routing
- ⚡ End-to-end workflow automation using n8n

---

# 🛠️ Tech Stack

- n8n
- Google Gemini
- Google Sheets API
- Google Calendar API
- AI Agent
- Structured Output Parser
- Simple Memory

---

# 📂 Workflow Overview

## Create Study Plan

```text
Chat Trigger
      │
      ▼
Intent Analyzer
      │
      ▼
Create Plan Agent
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

## Reschedule Study Plan

```text
Chat Trigger
      │
      ▼
Intent Analyzer
      │
      ▼
Read Study Sessions
      │
      ▼
Aggregate Sessions
      │
      ▼
AI Rescheduler
      │
      ▼
Update Google Sheets
      │
      ▼
Update Google Calendar
```

---

# 📌 Current Status

## ✅ Milestone 1 – AI Study Planner MVP

- AI-powered study schedule generation
- Google Gemini integration
- Structured JSON output
- Google Sheets integration

## ✅ Milestone 2 – Google Calendar Integration

- Automatic creation of study sessions
- Calendar synchronization
- Personalized scheduling

## 🚧 Milestone 3 – Intelligent Rescheduling *(In Progress)*

- Intent-based routing
- Aggregate existing study sessions
- AI-powered study session identification
- Automatic Sheet updates
- Automatic Calendar updates

---

# 💬 Example Commands

### Create a Study Plan

```
Generate a weekly timetable for Data Structures.
```

### Reschedule a Session

```
Shift my Ethics study session to Friday evening.
```

# 📁 Repository Structure

```text
ai-study-planner-agent/
│
├── README.md
├── workflows/
│   ├── create-study-plan.json
│   └── reschedule-study-plan.json
│
├── screenshots/
└── assets/
```

---

# 🚀 Future Improvements

- Smart conflict detection
- Automatic workload balancing
- Daily study reminders
- Email notifications
- WhatsApp / Telegram integration
- Weekly progress reports
- Study analytics dashboard
- PDF study plan export
- Voice-based study planner
- Live deployment

---

# 🎯 Learning Outcomes

This project demonstrates:

- AI Workflow Automation
- Prompt Engineering
- Google API Integration
- Workflow Automation with n8n
- Structured AI Outputs
- Event Synchronization
- AI-powered Scheduling
- Low-Code AI Development

---

# 👨‍💻 Author

**Karina Pandav**
