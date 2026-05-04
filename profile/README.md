# Apider

**Automation infrastructure for developers — without infrastructure.**

Apider is a cloud-native automation platform that allows developers to connect services like Email, Telegram, Discord, Slack, and Google Sheets using simple Python code — while execution, scaling, and security are handled entirely in the cloud.

---

## ⚡ What makes Apider different?

- **Code-first approach** — no YAML, no DSL, no config files  
- **One-liner integrations** — connect services instantly  
- **Cloud execution** — no servers, no cron jobs  
- **Thin SDK + powerful backend** — logic stays secure and scalable  

---

## 🚀 Example

```python
from apider import Email, Telegram, CloudScheduler

def monitor():
    emails = Email.read(unread_only=True)
    Telegram.send(f"📬 {len(emails)} new emails")

CloudScheduler.every_minutes(10, monitor)
```

✔ No infrastructure  
✔ No boilerplate  
✔ Just logic  

---

## 🧠 Mental Model

> "Zapier + AWS Lambda + Python SDK — unified into one system"

---

## 🛠️ Core Modules

- 📧 Email (SMTP/IMAP)  
- 📨 Telegram  
- 💬 Discord  
- 💼 Slack  
- 📊 Google Sheets (with type inference)  
- ⏰ Scheduler (cloud)  <!--(local + cloud) --> 

---

## 🌐 Ecosystem

- **SDK (PyPI):** `pip install apider`  
- **Website:** https://apider-io.github.io  
- **Source:** https://github.com/Apider-io/apider  

---

## 🔐 Architecture

Apider uses a **thin-client / cloud-runtime model**:

- The SDK is a lightweight proxy (published on PyPI)  
- Execution happens in a secure cloud environment  
- Backend logic is isolated and continuously upgradable  

---

## 🎯 Vision

Eliminate the friction between idea and execution.  

We believe developers should focus on **logic** — not infrastructure, OAuth, or deployment complexity.

---

## 🤝 Contributing

We welcome ideas, integrations, and improvements:

- Suggest new modules (WhatsApp, Webhooks, AI, etc.)  
- Open issues or discussions  
- Help expand the ecosystem  

---

## 📫 Contact

- **Website:** https://apider-io.github.io  
- **Email:** frostcore@jafa.dev  

---

*Built by Jorge de la Flor (FrostCore)*
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
