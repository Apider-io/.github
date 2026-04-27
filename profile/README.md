# Apider

**Redefining automation for developers and builders.**

Apider's mission is to eliminate the friction between idea and execution — letting any developer connect complex services with a single line of Python and scale to the cloud instantly.

---

## 🛠️ Projects

<!--### [Apider SDK](https://github.com/Apider-io/apider)-->
### Apider SDK

The core of our ecosystem. A Python thin-client SDK that abstracts the complexity of APIs like Google Sheets, Telegram, Discord, Slack, and Email (SMTP/IMAP).

- **Approach:** Code-first. No YAML, no DSL, no config files.
- **Architecture:** Thin client on PyPI → execution on Azure Functions.
- **Status:** ✅ Live on PyPI — `pip install apider`

```python
from apider import Email, Telegram, CloudScheduler

def monitor():
    emails = Email.read(unread_only=True)
    Telegram.send(f"📬 {len(emails)} new emails")

CloudScheduler.every_minutes(10, monitor)
```

---

## ✨ Philosophy

At Apider we believe the value of a developer is in their logic — not in fighting OAuth configurations or maintaining servers.

- **IP Protection:** Your code runs in an isolated, secure environment. The PyPI package contains no integration logic — just HTTP calls.
- **Simplicity:** If it takes more than one line to send a message or read a table, it's not Apider.
- **Scalability:** From a local script to a scheduled cloud job in seconds.

---

## 💳 Plans

| Plan | Price | Executions/month | Jobs |
|---|---|---|---|
| Free | $0 | 2,000 | 1 |
| Pro | $19/mo | 50,000 | 10 |
| Business | $49/mo | 500,000 | Unlimited |

[→ Get started](https://apider-io.github.io)

---

## 🤝 Community & Contributions

The execution core is private to guarantee service security, but the SDK is **visible and auditable**. We believe in software transparency.

- **Developer?** Review the SDK and help us improve modules.
- **Have an idea?** Open an Issue with a new module proposal (WhatsApp, Webhooks, AI, etc.).

---

## 📫 Contact & Support

- **Website:** [apider-io.github.io](https://apider-io.github.io)
- **PyPI:** [pypi.org/project/apider](https://pypi.org/project/apider/)
- **Email:** [frostcore@jafa.dev](mailto:frostcore@jafa.dev)

---

*Built with ❤️ by [Jorge de la Flor](https://github.com/Jorge-de-la-Flor)*

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
