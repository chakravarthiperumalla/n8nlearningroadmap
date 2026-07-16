# 🤖 AI Learning Roadmap Generator (n8n Workflow)

Generate a personalized AI-powered learning roadmap for any topic using **n8n**, **Google Gemini AI**, and **Gmail**.

This workflow collects user input through an n8n form, generates a complete day-by-day learning roadmap using Google Gemini, converts it into an HTML file, and automatically emails it to the user.

---

## ✨ Features

- 📚 Generate customized learning roadmaps for any topic
- 🎯 Supports Beginner, Intermediate, and Advanced learners
- 📅 User-defined learning duration (up to 180 days)
- ⏰ Customize study hours per day
- 📝 Includes:
  - Daily lessons
  - Practice exercises
  - Assignments
  - Daily quizzes with answers
- 🏆 Final capstone project
- 📖 Recommended learning resources
- 📧 Automatically emails the roadmap to the user
- 🌐 Outputs a beautifully formatted HTML document

---

## 🛠️ Tech Stack

- **n8n**
- **Google Gemini API**
- **Gmail API**
- JavaScript (Code Node)
- HTML

---

## 📋 Workflow Overview

```text
Form Trigger
      │
      ▼
Edit Fields
      │
      ▼
Validate Duration
      │
      ├──────────────► Invalid Input (Stop)
      │
      ▼
Google Gemini AI
      │
      ▼
Generate Learning Roadmap
      │
      ▼
Build HTML Attachment
      │
      ▼
Send Email
```

---

## 📥 User Inputs

The workflow collects the following information:

| Field | Type |
|--------|------|
| Topic | Text |
| Duration (Days) | Number |
| Learning Level | Beginner / Intermediate / Advanced |
| Hours Per Day | Number |
| Output Format | PDF / Markdown / DOCX *(Currently generates HTML)* |
| Email Address | Text |

---

## 📤 Output

The generated roadmap includes:

- Introduction
- Course Overview
- Day-by-day Learning Plan
- Lessons
- Practical Exercises
- Assignments
- Daily Quiz
- Quiz Answers
- Module Breakdown
- Final Capstone Project
- Learning Resources

The roadmap is generated as an **HTML file** and emailed directly to the user.

---

## ⚙️ Prerequisites

Before using this workflow, configure:

- Google Gemini API credentials
- Gmail OAuth credentials
- n8n instance

---

## 🔑 Required Credentials

### Google Gemini

- API Key

### Gmail

- OAuth2 Authentication

---

## 🚀 Installation

1. Clone this repository.

```bash
git clone https://github.com/yourusername/ai-learning-roadmap-generator.git
```

2. Open n8n.

3. Import the workflow JSON.

4. Configure:

- Google Gemini credentials
- Gmail credentials

5. Activate the workflow.

6. Open the generated Form URL.

---

## 🧠 How It Works

1. User fills out the form.
2. Workflow validates the learning duration.
3. Google Gemini generates a complete curriculum.
4. HTML content is cleaned and converted into a downloadable file.
5. The HTML file is attached to an email.
6. User receives the personalized roadmap.

---

## 📁 Project Structure

```
AI Learning Roadmap Generator.json
README.md
```

---

## 📌 Validation Rules

- Duration must be greater than **0**
- Maximum duration is **180 days**

Invalid requests stop automatically.

---

## 📸 Workflow

Import the workflow into n8n to view the complete visual automation.

---

## 🔮 Future Improvements

- PDF generation
- DOCX export
- Markdown export
- Progress tracking
- Daily reminder emails
- Notion integration
- Google Drive storage
- Learning analytics dashboard

---

## 🤝 Contributions

Contributions, issues, and feature requests are welcome!

Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Perumalla Chakravarthi**

If you found this project helpful, don't forget to ⭐ the repository.
