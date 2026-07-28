# 🎓 AI Study Planner Agent

An AI-powered Study Planner built using **n8n**, **Google Gemini/Groq**, **Google Sheets**, and **Google Calendar**. The assistant generates personalized study schedules, stores them in Google Sheets, creates Google Calendar events, and intelligently reschedules study sessions using natural language.

This project demonstrates how AI agents can automate real-world productivity workflows through conversational interfaces and workflow automation.

---

# ✨ Features

## 📅 AI Study Plan Generation
- Generate personalized study plans based on exam details
- Automatically divide syllabus into multiple study sessions
- Prioritize topics based on importance
- Produce structured JSON outputs for downstream automation

---

## 🤖 Conversational AI Agent
- Chat-based interaction
- Understands natural language requests
- Supports multiple study-related commands
- Maintains conversation context

Example:

> "Create a study plan for my DBMS exam."

---

## 🎯 AI Intent Classification

Automatically classifies user requests into:

- Create Study Plan
- Reschedule Study Session

This enables a single chatbot to intelligently route requests to different workflows.

---

## 🔄 Intelligent Study Session Rescheduler

Users can modify their study plans using natural language.

Examples:

- Reschedule my Calculus session.
- Move tomorrow's DBMS session to Friday.
- Shift my Mathematics session to 2 PM.

The AI automatically:

- Reads existing study sessions
- Identifies the correct session
- Generates the updated schedule
- Updates Google Sheets
- Synchronizes Google Calendar

---

## 📊 Google Sheets Integration

Automatically maintains study data.

### Plans Sheet

Stores:

- Plan ID
- Exam Name
- Start Date
- Exam Date
- Created Timestamp

### Sessions Sheet

Stores:

- Plan ID
- Date
- Start Time
- End Time
- Subject
- Topic
- Priority
- Status
- Calendar Event ID

---

## 📅 Google Calendar Integration

Automatically:

- Creates calendar events
- Updates events after rescheduling
- Keeps study sessions synchronized

---

## 📋 Structured AI Outputs

Uses Structured Output Parser to guarantee valid JSON responses.


# 🛠 Tech Stack

### Workflow Automation

- n8n

### AI

- Google Gemini *(or Groq GPT-OSS Models)*

### Google Services

- Google Sheets API
- Google Calendar API
- Google OAuth2

### AI Components

- AI Agent
- Intent Classifier
- Structured Output Parser
- Simple Memory

---

# 🏗 Workflow Architecture

## Create Study Plan

```text
                    User
                      │
                      ▼
                Chat Trigger
                      │
                      ▼
             Intent Classifier
                      │
                      ▼
             AI Study Planner
                      │
                      ▼
         Structured Output Parser
                      │
            ┌─────────┴─────────┐
            ▼                   ▼
      Google Sheets      Google Calendar
                      │
                      ▼
              Respond to User
```

---

## Reschedule Study Plan

```text
                    User
                      │
                      ▼
                Chat Trigger
                      │
                      ▼
             Intent Classifier
                      │
                      ▼
             Read Google Sheets
                      │
                      ▼
             Aggregate Sessions
                      │
                      ▼
       Merge Chat + Session Data
                      │
                      ▼
             AI Rescheduler
                      │
                      ▼
         Structured Output Parser
                      │
              Update Google Sheets
                      │
                      ▼
            Update Google Calendar
                      │
                      ▼
               Respond to User
```

---

# 💬 Example Commands

## Create a Study Plan

```
Create a study plan for my Data Structures exam.
```

```
Generate a weekly timetable for Machine Learning.
```

---

## Reschedule a Session

```
Move my Calculus study session to tomorrow at 2 PM.
```

```
Shift my DBMS revision to Friday evening.
```

```
Reschedule my Mathematics session.
```

---

# 🚀 Current Status

## ✅ Completed

- AI-powered Study Plan Generation
- Conversational AI Agent
- Intent Classification
- Google Sheets Integration
- Google Calendar Integration
- Structured Output Parsing
- AI-powered Study Session Rescheduling
- Google Sheets Synchronization
- Google Calendar Synchronization
- End-to-End Workflow Automation

---

## 🚧 Planned Enhancements

- Unique Session IDs
- Study Conflict Detection
- Automatic Workload Balancing
- Daily Study Reminders
- Email Notifications
- WhatsApp / Telegram Integration
- Weekly Progress Reports
- Study Analytics Dashboard
- PDF Study Plan Export
- Voice-enabled Study Planner
- Deployment

---

# 📚 Learning Outcomes

This project demonstrates practical experience with:

- AI Workflow Automation
- Prompt Engineering
- AI Agents
- Intent Classification
- Structured AI Outputs
- Workflow Orchestration using n8n
- Google Sheets API
- Google Calendar API
- Data Aggregation
- Data Merging
- JSON Processing
- Event Synchronization
- Conversational AI
- Low-Code AI Development

---

# 🚀 Future Roadmap

- Multi-user authentication
- User-specific study plans
- Adaptive scheduling using AI
- Exam progress tracking
- Revision optimization
- Mobile app integration
- Dashboard with analytics
- RAG-powered syllabus understanding
- Voice assistant support

---

# 🤝 Contributing

Contributions, suggestions, and feature requests are welcome.

Feel free to fork this repository and submit a pull request.

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Karina Pandav**

If you found this project helpful, consider giving it a ⭐ on GitHub.
