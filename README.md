# 🏥 Hospital AI Reception Chatbot

**An AI-assisted hospital reception chatbot with urgency assessment, patient guidance, and human escalation.**

**Day 5 Mini Project — AI-Assisted Hospital Workflow**

This project demonstrates how a browser-based AI chatbot can support hospital reception by collecting symptom information, answering common questions, providing general guidance, and flagging cases that require human attention.

Built using plain HTML, CSS, and JavaScript, with the Claude API for AI-powered responses.
## 📸 Application Screenshot

![Hospital AI Chatbot](Hospital%20AI%20Reception%20Chatbot.png)

## ✨ Features

- 💬 **AI Reception Chat** — Interact with an AI assistant through a conversational interface.
- 🩺 **Symptom Collection** — Collect basic information about a patient's reported symptoms.
- 🚦 **Urgency Assessment** — Demonstrate a proposed urgency scoring system from Level 1 to Level 5.
- ⏱️ **Wait-Time Estimates** — Provide indicative waiting-time information where appropriate.
- ❓ **FAQs and Directions** — Help users find general hospital information and directions.
- 👨‍⚕️ **Human Escalation** — Flag potentially urgent conversations for review by qualified hospital staff.
- 🏥 **Human-Centered Workflow** — Keep clinical examinations, diagnoses, and treatment decisions under qualified healthcare professionals.

## 🔄 Human–AI Workflow

| Task | Responsibility |
|---|---|
| Collect reported symptoms | AI-assisted |
| Preliminary urgency assessment | AI-assisted, requiring appropriate validation |
| General waiting-time information | AI-assisted, based on available information |
| FAQs and directions | AI-assisted |
| Flag potentially critical cases | AI flags; trained human staff respond |
| Clinical examination | Qualified healthcare professional |
| Diagnosis and treatment | Qualified healthcare professional |

**Important:** An AI-generated urgency score is not a clinically validated triage decision. A real hospital deployment requires clinical oversight, validated protocols, appropriate testing, and reliable escalation procedures.

## 🛠️ Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **AI:** Claude via the Anthropic API
- **Architecture:** Static web application
- **Dependencies:** No frontend framework or build process required

## 🚀 Getting Started

### 1. Clone the repository

Replace `YOUR_GITHUB_USERNAME` with your GitHub username and `YOUR_REPOSITORY_NAME` with the repository's actual name.

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME
```

### 2. Open the application

If the repository contains an `index.html` file, you can open it in your browser or run a local development server:

```bash
python -m http.server 8000
```

Then visit:

http://localhost:8000

Python is needed only for this optional local server, not for the application itself.

### 3. Configure the AI API

The chatbot uses the Anthropic API to generate AI responses.

If the application currently calls Claude directly from browser-side JavaScript, do not place a real API key in `index.html`, JavaScript files, or a public GitHub repository.

For secure deployment, use a backend service to store the API key and make authenticated API requests. Configure the API key as a server-side environment variable.

## 🌐 Deployment with GitHub Pages

If the application works entirely as a static frontend without requiring a secure backend, you can publish it using GitHub Pages.

1. Open your GitHub repository.
2. Go to **Settings → Pages**.
3. Under the build and deployment settings, select **Deploy from a branch**.
4. Select the `main` branch and the root (`/`) folder if `index.html` is in the repository root.
5. Click **Save** and wait for the deployment to complete.

GitHub will provide a published website URL in the Pages settings.

**Note:** GitHub Pages cannot run backend code or securely protect an Anthropic API key. If the chatbot needs Claude API access in production, deploy the frontend and a secure backend separately.

## 🔐 Privacy and Security

- Collect only the information needed for the chatbot's intended purpose.
- Do not commit API keys, credentials, or patient information to GitHub.
- Avoid sending identifiable patient or medical information to external AI services without appropriate authorization and privacy safeguards.
- Protect any backend endpoints against unauthorized use.
- Make the system's AI limitations clear to users.
- Ensure urgent cases have a clear route to human assistance.

## ⚠️ Healthcare Disclaimer

This project is an educational demonstration of an AI-assisted hospital reception workflow. It is not a substitute for emergency services, professional medical advice, clinical triage, diagnosis, or treatment.

Users with potentially life-threatening symptoms should be directed to emergency services or qualified healthcare professionals immediately. AI-generated assessments must not delay urgent care.

## 📄 License

This project is intended to use the MIT License. See the `LICENSE` file in the repository for the full license text.

---

Developed as a mini project on AI-assisted hospital workflows.
