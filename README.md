# ThinkLessX – Telegram AI Decision Bot

![n8n](https://img.shields.io/badge/n8n-Workflow-orange)
![Telegram](https://img.shields.io/badge/Telegram-Bot-blue)
![AI](https://img.shields.io/badge/AI-Decision%20Engine-purple)
![LLM](https://img.shields.io/badge/LLM-Local%20%2F%20Cloud-green)
![Status](https://img.shields.io/badge/Status-Production--Ready-success)

---

## 🧠 Overview

**ThinkLessX** is an intent-aware Telegram AI bot designed to eliminate *decision debt*. Instead of overwhelming users with summaries or suggestions, it converts incoming messages, documents, and media into **clear next actions**.

This project demonstrates a real-world, production-grade **n8n automation** that combines:

* multi-source text extraction
* AI-powered text unification
* intent & sentiment detection
* decision-first responses delivered directly on Telegram

---

## 🤖 Telegram Bot (Live Demo)

🔗 **Bot Link:** [https://t.me/ThinkLessX_bot](https://t.me/ThinkLessX_bot)

**Note:**
This bot is running on a **locally self-hosted n8n setup** (not a VPS).
Since it relies on **HTTPS tunneling** for external access, the bot may not always be online.

If you test the bot and it’s inactive, please **notify me via LinkedIn only**, and I’ll bring it online for you 😊
Your feedback and testing support are highly appreciated.

📬 **Contact:**

* LinkedIn: www.linkedin.com/in/omkar-sawant-953b47281
---

## 🚀 What This Automation Does

* Listens to incoming Telegram messages (text, images, PDFs, files)
* Automatically detects the input type
* Extracts readable text from:

  * images (OCR)
  * PDFs
  * TXT files
  * raw messages
* Cleans and unifies text into a single coherent block
* Understands **intent**, **sentiment**, and **urgency**
* Decides what the user should do next:

  * Act now
  * Store for reference
  * Defer
  * Ignore
  * Think later
* Sends a **clear, human-friendly reply** back to the user

No dashboards. No task lists. Just decisions, closed.

---

## 🧩 High-Level Workflow

```
Telegram Message
   ↓
Input Type Router
   ↓
Multi-Source Text Extraction Engine
   ↓
Text Unification Engine
   ↓
Intent & Decision Engine
   ↓
Telegram Decision Reply
```
### 🖼️ Automation Workflow:
![Workflow Screenshot](assets/workflow-diagram.png)


### 🖼️ Generated results:
![mailed Screenshot](assets/bot_response_2.png)

![mailed Screenshot](assets/bot_response_1.png)

---

## 🛠 Tech Stack

* **n8n** – Workflow orchestration & automation
* **Telegram Bot API** – User interaction layer
* **OCR API** – Text extraction from images
* **PDF/Text Extractors** – Document processing
* **LLMs (Local or Cloud)** –

  * Text Unification Agent
  * Intent & Decision Agent
* **Cohere / Local LLaMA** – Decision reasoning (pluggable)

This setup is fully modular and can run with **local LLMs** or **cloud-based models**.

---

## 📂 Folder Structure

```
ThinkLessX/
├── workflows/
│      └── ThinkLessX.json
│
├── prompts/
│   ├── text-unification-prompt.txt
│   └── decision-engine-prompt.txt
│
├── assets/
│   ├── workflow-diagram.png
│   └── bot-logo.png
│
├── README.md
└── LICENSE
```

---

## ⚙️ Setup Overview

1. Clone this repository
2. Import workflows into **n8n**
3. Create and configure a Telegram Bot token
4. Add API keys for OCR / LLM providers (or connect local LLMs)
5. Update environment variables in n8n
6. Activate the workflow

Once live, the bot immediately starts converting messages into decisions.

---

## 🎯 Example Use Cases

* 📄 Certificates & documents → *Store for reference*
* 📧 Joining letters & instructions → *Act now*
* 😤 Emotional messages → *Clarify intent & guide next step*
* 🔔 Notifications → *Ignore or think later*
* 🧠 Personal knowledge intake → *Decision-first processing*

This is ideal for:

* founders
* engineers
* students
* automation builders
* anyone overwhelmed by incoming information

---

## 🤝 Connect

If you’re working with **n8n**, **AI workflows**, **automation**, or **local LLMs**, feel free to connect.

🔗 This project is also featured on my **LinkedIn Projects** section.

Let’s build decision-first systems together.

---

## 📜 License

This project is open for learning and inspiration. Please credit the author if you reuse or adapt significant parts of the workflow.
