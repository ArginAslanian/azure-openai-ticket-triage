# 🚀 AI-Powered SecOps & IT Help Desk Triage Pipeline 🚨

## 📌 Project Overview
This project is a 100% serverless, AI-driven automation pipeline built to streamline front-line IT ticket handling. I created this architecture to solve a major operational bottleneck: the manual triage of support requests and security alerts. 

By intercepting incoming support emails and utilizing Azure OpenAI (gpt-4o-mini) to intelligently analyze, categorize, and assign urgency to the issues, this system instantly routes structured ChatOps alerts directly to an operations center. It bridges standard IT support with modern Information Systems Engineering and SecOps workflows to drastically reduce response times.

---

## 🏗️ Architecture & Technologies Used
* ☁️ **Microsoft Azure Logic Apps:** Serverless workflow orchestration engine.
* 🧠 **Azure OpenAI Service (gpt-4o-mini):** Advanced natural language processing and ticket categorization.
* 📧 **Microsoft Outlook/Exchange:** Ingestion endpoint for capturing end-user support emails.
* 💬 **Slack API:** ChatOps destination for pushing instant, structured alerts to the team.
* 🧹 **HTML to Text Conversion:** Data sanitization to strip raw HTML and optimize AI payloads.

---

## ⚙️ How It Works (The Workflow)
1. **Ingestion:** An end-user sends an email to the designated help desk inbox.
2. **Trigger:** Azure Logic Apps detects the incoming email and triggers the pipeline.
3. **Data Sanitization:** The messy HTML email body is converted into clean plain text.
4. **AI Triage & Analysis:** The sanitized text is securely passed to Azure OpenAI. The model determines the **Category**, the **Urgency**, and drafts an immediate **Mitigation Action**.
5. **ChatOps Routing:** The structured AI response and original ticket details are pushed via API into a dedicated Slack channel (`#it-ticket-alerts`).

---

## 📸 Project Showcase & Build Journey

### 1. Azure OpenAI Model Deployment
<img width="1885" height="907" alt="gpt-4o-mini deployment" src="https://github.com/user-attachments/assets/466aa7ee-5257-45fa-83a3-f2d786e2f74a" />

### 2. Logic App Workflow & AI Connection
<img width="1891" height="892" alt="openai prompts" src="https://github.com/user-attachments/assets/d87221cc-e458-4a26-9c5d-feb9a6ebcfce" />

### 3. Data Sanitization (HTML to Text)
<img width="1901" height="912" alt="Formatting fix" src="https://github.com/user-attachments/assets/d770afea-8fdd-4a72-a979-98b82005be43" />

### 4. Slack API Integration
<img width="1907" height="909" alt="Slack Connection" src="https://github.com/user-attachments/assets/82a9b5fc-76c3-410b-ac0f-579a789fc9cb" />

### 5. Final Output: Real-Time ChatOps Alert! 🎉
<img width="1396" height="516" alt="Slack message from Logic Apps" src="https://github.com/user-attachments/assets/9a8cc6be-9c32-4ca7-b0b8-464c9cb5d970" />

