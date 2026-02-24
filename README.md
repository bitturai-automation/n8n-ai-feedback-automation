# 🚀 AI-Powered Customer Feedback Automation System

## 📌 Overview

This project is a real-world AI automation system built using n8n and OpenAI.

The system collects customer feedback through a form, uses an AI Agent to classify the feedback, and automatically routes it to the correct database and communication channels.

This workflow demonstrates advanced LLM-based classification, conditional routing, database automation, and multi-platform integration.

---

## 🏗 System Architecture

Form Submission  
→ AI Agent (LLM Classification)  
→ Merge Node  
→ Switch Node (Conditional Routing)

### Routing Logic:

If **Complain**:
- Store record in Airtable (Complain Table)
- Send Slack notification
- Send automated Gmail response

If **Compliment**:
- Store record in Airtable (Compliment Table)

If **Feature Addition Request**:
- Store record in Airtable (Feature Request Table)
- Send Slack notification

---

## 🤖 AI Classification Logic

The AI Agent categorizes feedback into one of the following:

- Complain  
- Compliment  
- Feature Addition Request  

The classification is controlled using prompt-based logic and OpenAI GPT model.

---

## 🛠 Tech Stack

- n8n (Workflow Automation)
- OpenAI GPT-4.1-nano
- LangChain AI Agent Node
- Airtable (Database Storage)
- Slack API Integration
- Gmail Automation
- Conditional Switch Routing

---

## 📥 Form Fields

- Full Name
- Email Address
- Contact Number
- Feedback Message

---

## 🔄 Automation Flow

1. User submits feedback via n8n form.
2. AI Agent analyzes and classifies feedback.
3. Switch node routes data based on classification.
4. Airtable stores structured record.
5. Slack alerts are triggered (where required).
6. Gmail auto-response is sent for complaints.

---

## 🎯 Key Features

- LLM-powered feedback classification
- Multi-branch conditional routing
- Structured database automation
- Automated Slack alerts
- Automated Gmail response system
- Scalable AI workflow architecture

---

## 📊 Business Impact

- Eliminates manual feedback sorting
- Reduces response time
- Automates internal communication
- Improves data organization
- Reduces operational overhead

---

## 🚀 Real-World Use Cases

- SaaS feedback automation
- Startup support system
- AI-powered complaint management
- Intelligent workflow routing
- Internal operations automation

---

## 🔮 Future Enhancements

- Add sentiment scoring
- Add priority tagging
- CRM integration
- Analytics dashboard
- API deployment for SaaS usage

---

## 📂 Repository Contents

- Feedback form.json → n8n workflow export
- README.md → Documentation

---

## 👨‍💻 Author

Bittu Rai  
AI Automation Engineer  
GitHub: https://github.com/bitturai-automation  
LinkedIn: https://linkedin.com/in/bitturai  

---

⭐ Star this repository if you found it useful.
