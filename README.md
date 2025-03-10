# 🚀 AIpplyon - AI Job Application Agent Chrome Extension

**AIpplyon** is an AI-powered Chrome extension designed to fully automate and optimize the job application process. It integrates **AutoGen for job analysis** and **CrewAI for automation**, ensuring users have **100% manual control** over resume updates, applications, and recruiter outreach.

---

## 🌟 Features
- ✅ **AI Resume Optimization** – ATS-friendly resume suggestions.
- ✅ **Automated Job Applications** – Auto-fills forms on LinkedIn, Indeed, Glassdoor, etc.
- ✅ **Recruiter Messaging Automation** – Personalized LinkedIn & email outreach.
- ✅ **Job Tracking & Notifications** – Logs applications in Google Drive & sends alerts.
- ✅ **Weekly AI Fine-Tuning** – Continuously improves based on user feedback.

---

## 📂 GitHub Repository Structure

AIpplyon/ ├── backend/ # FastAPI backend │ ├── api/ # API endpoints for AI processing │ │ ├── resume_optimizer.py │ │ ├── job_analysis.py │ │ ├── automation.py │ │ ├── rag_retrieval.py │ ├── auth/ # User authentication (Google OAuth) │ │ ├── google_oauth.py │ ├── tests/ # Unit & integration tests │ │ ├── test_api.py │ │ ├── test_resume_optimizer.py │ │ ├── test_automation.py │ ├── main.py # FastAPI app entry point │ ├── requirements.txt # Python dependencies │ ├── chrome_extension/ # Chrome Extension UI │ ├── manifest.json # Chrome extension manifest │ ├── scripts/ # JavaScript logic │ │ ├── background.js │ │ ├── content.js │ │ ├── popup.js │ ├── styles/ # Chatbot styling │ │ ├── style.css │ ├── popup.html # Chatbot interface │ ├── models/ # AI model fine-tuning & storage │ ├── fine_tuning/ │ │ ├── weekly_finetune.py │ │ └── training_data/ │ ├── .github/ # GitHub Actions CI/CD workflows │ ├── workflows/ │ │ ├── ci-cd.yml │ ├── docs/ # Documentation │ ├── CONTRIBUTING.md │ ├── API_Documentation.md │ ├── README.md # Project Overview └── .gitignore # Ignore unnecessary files


---

## 📌 Phase-wise Implementation Plan

### 🚀 **Phase 1: Chrome Extension UI & Authentication (Day 1-2)**
- 🔹 Setup Chrome extension with **Google OAuth login**.
- 🔹 Develop **chatbot UI for job analysis**.

### 🚀 **Phase 2: AI Resume Optimization with AutoGen (Day 3-4)**
- 🔹 Implement **ATS analysis & resume optimization**.
- 🔹 Provide **manual editing for AI-generated content**.

### 🚀 **Phase 3: CrewAI for Job Automation (Day 5-6)**
- 🔹 Automate **job application form filling**.
- 🔹 Automate **LinkedIn & recruiter email messaging**.

### 🚀 **Phase 4: Job Tracking & Notifications (Day 7-8)**
- 🔹 Implement **job tracking in Google Sheets**.
- 🔹 Send **automated email notifications** for updates.

### 🚀 **Phase 5: AI Fine-Tuning on GCP (Day 9-10)**
- 🔹 **Weekly AI model fine-tuning** based on user data.

### 🚀 **Phase 6: Testing, Debugging & Deployment (Day 11-14)**
- 🔹 **Real-world testing on LinkedIn, Indeed, Glassdoor**.
- 🔹 **Debugging & UI/UX improvements**.
- 🔹 **Deployment to Chrome Web Store**.
- 🔹 **Integrate donation ('Buy Me a Coffee') link**.

---

## 🛠️ Tech Stack
- **Frontend:** Chrome Extension (JavaScript, Manifest V3)
- **Backend:** FastAPI (Python), PostgreSQL
- **AI Models:** GPT-4, Mixtral, LLaMA, Mistral
- **Automation:** Playwright, Selenium, AutoGen, CrewAI
- **Cloud Infrastructure:** Google Cloud Platform (GCP)
- **Storage:** Google Drive API, Sheets API

---

## 🛠 Installation Instructions

```bash
git clone https://github.com/yourusername/AIpplyon.git
cd AIpplyon/backend
pip install -r requirements.txt
uvicorn main:app --reload
