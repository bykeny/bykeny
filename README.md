## Hey, I'm Kanan

I build backends in .NET: APIs, data models, and the boring-but-important parts that keep apps running. I like it when things are well-structured, tested, and easy to deploy.

I'm currently doing my MSc in Software Engineering at the **University of Tartu** 🇪🇪, and I'm looking for a **junior .NET / full-stack role or internship** in Estonia or remote.

---

### What I work with

**Daily:** C#, ASP.NET Core (Minimal API, Web API, MVC), EF Core, PostgreSQL, MS SQL
**Real-time & auth:** SignalR, JWT with rotating refresh tokens
**Frontend:** React, React Native (Expo), Next.js, Blazor, TypeScript
**Shipping it:** Docker, GitHub Actions, Azure, Terraform
**Also used:** ML.NET, LLM tool calling, PayPal APIs

---

### Projects worth a look

**[TiltGuard](https://github.com/bykeny/TiltGuard)**: real-time tilt detection and cooldown coaching for competitive gamers *(in progress)*
.NET 10 Minimal API · EF Core · PostgreSQL · SignalR · React Native (Expo) · Docker · GitHub Actions
When you're on a losing streak and getting angrier each game, you usually keep queuing. TiltGuard scores your recent matches and, if the risk is high, locks you into a cooldown that the server enforces, so you can't just tap past it. The parts I'm proudest of:
- a weighted tilt score over your last 5 matches, plus hard override rules for really bad patterns
- the API returns `423 Locked` during a cooldown, and a background service releases expired locks
- rotating refresh tokens with reuse detection, and idempotent subscription webhooks
- a CI pipeline that builds, health-checks the Docker image, and deploys over SSH

**[Allowance](https://github.com/bykeny/allowance)**: spending rules for AI agents, built at the PayPal AI Hackathon · [live demo](https://allowance-g8sh.onrender.com/)
Next.js · TypeScript · PayPal Orders & Vault APIs · LLM tool calling
Nobody hands an AI agent a credit card, so this gives it a budget with rules instead. Every purchase request gets **allowed** (paid automatically), **escalated** (a human approves it in PayPal checkout), or **denied**. The key design choice is that the LLM never talks to PayPal. A deterministic policy engine makes the decision, and every request ends up in an audit ledger.
*(The demo runs in sandbox mode on a free instance, so give it a minute to wake up.)*

**[Streakly](https://github.com/bykeny/Streakly)**: habit and goal tracker with AI-generated insights
ASP.NET Core MVC · EF Core · AI integration
I built this to practice a full app end to end: auth, data modeling, and turning raw habit data into suggestions that are actually useful.

**[spam-detector](https://github.com/bykeny/spam-detector)**: spam classifier built on ML.NET
ML.NET · ASP.NET Core API · TypeScript frontend
Binary text classification trained and served entirely in .NET. A small project, but it shows ML doesn't have to mean Python.

---

### Team projects (private repos, happy to talk about them)

- **AI agent auditability PoC**: university software project with real clients. We're building a way to trace and audit what AI agents actually do.

---

### Right now I'm...

- 🛡️ building TiltGuard toward its first release
- 🎓 picking and starting my master's thesis
- 🤖 working on the AI agent auditability project
- 🎮 building *Escape the Maze*, a WebGL car maze game, for a computer graphics course

---

### Get in touch

If you're hiring juniors, working on something interesting in .NET, or just want to talk code, reach out.

💼 [LinkedIn](https://www.linkedin.com/in/kananramazanov)
📧 kenanramaznov@gmail.com
📍 Tartu, Estonia · open to Tallinn and remote
