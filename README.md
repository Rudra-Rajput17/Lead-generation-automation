# 🚀 AI Lead Generation & Chatbot Automation System

## 📌 Overview

This project is an end-to-end **AI-powered lead generation and qualification system** built using automation tools and LLMs. It automatically:

- Extracts leads from platforms (LinkedIn, Email, etc.)
- Uses AI to classify leads (Hot / Warm / Cold)
- Stores and manages leads in a CRM (Airtable)
- Engages users through an AI chatbot
- Automates follow-ups via Email/WhatsApp

---

## 🧠 Key Features

### 🔍 Lead Extraction

- Scrapes or collects leads from:
  - LinkedIn (via automation tools)
  - Email inbox
  - Web forms / chatbot

### 🤖 AI Lead Qualification

- Uses LLMs to:
  - Understand user intent
  - Classify leads into:
    - 🔥 Hot Leads
    - 🌤 Warm Leads
    - ❄ Cold Leads

### 💬 AI Chatbot

- Custom chatbot workflow
- Maintains conversation context
- Stores chat history (memory)
- Can extract useful data (name, email, phone)

### 🗂 CRM Integration

- Stores leads in Airtable
- Fields include:
  - Name
  - Email
  - Phone
  - Lead Score
  - Conversation Data

### ⚡ Automation Workflows (n8n)

- Trigger-based workflows
- Webhook integrations
- Conditional routing
- Data transformation

### 📩 Automated Follow-ups

- Hot leads → sent directly to sales
- Warm leads → nurture campaigns
- Cold leads → stored for later

---

## 🏗️ System Architecture

This project is divided into **4 core workflows**:

### 1️⃣ PhantomBuster Lead Collector

- Extracts leads from LinkedIn and other sources
- Uses automation tools like PhantomBuster
- Sends data to n8n via webhook

### 2️⃣ ICP Scorer + AI Qualifier

- Scores leads based on Ideal Customer Profile (ICP)
- Uses LLM (Groq/OpenAI) for qualification
- Classifies leads into Hot / Warm / Cold

### 3️⃣ Outreach + Follow-up Automation

- Sends personalized emails/messages
- Automates follow-ups based on lead category
- Integrates with Email/WhatsApp APIs

### 4️⃣ Chatbot App (Live)

- Interactive chatbot for capturing leads
- Maintains conversation memory
- Extracts structured data (name, email, phone)
- Directly feeds data into the system

### 🔄 Overall Flow

1. Lead Collection (PhantomBuster / Chatbot)
2. Webhook Trigger (n8n)
3. ICP Scoring + AI Qualification
4. Airtable Storage
5. Outreach & Follow-up Automation

---

## 🛠️ Tech Stack

- **Automation**: n8n
- **AI/LLM**: OpenAI / LLM APIs
- **Database/CRM**: Airtable
- **Scraping Tools**: PhantomBuster / Apify
- **Communication**: Email APIs / WhatsApp APIs

---

## 📂 Project Structure

```
├── workflows/
│   ├── 01-phantombuster-lead-collector.json
│   ├── 02-icp-scorer-groq-qualifier.json
│   ├── 03-outreach-followup.json
│   └── 04-chatbot-app.json
│
└── README.md
```

├── workflows/
│ ├── chatbot-workflow.json
│ ├── lead-classification.json
│ └── email-automation.json
│
├── docs/
│ └── architecture.png
│
├── scripts/
│ └── data-processing.js
│
└── README.md

````

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
````

### 2. Setup n8n

- Install n8n (Docker or local)
- Import workflows from `/workflows`

### 3. Configure Environment Variables

- Groq API Key
- Airtable API Key
- Email credentials

### 4. Run Workflows

- Start n8n
- Activate workflows
- Test using webhook URLs

---

## 📊 Example Use Case

1. A user sends a message via chatbot
2. Chatbot captures:
   - Name
   - Email
   - Phone

3. LLM analyzes intent
4. Lead is classified as "Hot"
5. Data stored in Airtable
6. Sales team gets notified instantly

---

## 🚀 Future Improvements

- Add vector database for long-term memory
- Improve lead scoring with ML models
- Add multi-language chatbot support
- Dashboard for analytics (Power BI / Streamlit)

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 📬 Contact

For queries or collaboration:

- Email: rrudra3404@gmail.com
- LinkedIn: www.linkedin.com/in/rudra-pratap-singh-59122a24b

---

## ⭐ If you like this project

Give it a star on GitHub ⭐ and share it!
