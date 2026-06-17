#  Ripple - Daily Habit Tracker

> Small habits, big waves.

![Platform](https://img.shields.io/badge/Platform-CTO.ai-blueviolet?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-blue?style=flat-square)

---

##  Overview

**Ripple** is a personal habit tracking app built on the [CTO.ai](https://cto.ai) platform. Just like a ripple in water, small consistent actions spread outward , creating waves of lasting change in your life.

Whether you're building a morning routine, staying consistent at the gym, or cultivating mindfulness, Ripple keeps you accountable every single day.

---

##  Architecture & Tech Stack

This project was built to stress-test full-lifecycle software engineering ownership—bridging application development with automated GitOps delivery pipelines.

| Technology | Purpose |
| :--- | :--- |
| **CTO.ai** | App platform, environment hosting, and workflow automation |
| **JavaScript / Node.js** | Core asynchronous application logic and state management |
| **CTO.ai SDK** | CLI automation, secrets handling, and pipeline integration |
| **Markdown** | Technical documentation and system architecture mapping |

---

##  Key Features

* **Automated CI/CD:** Continuous delivery pipeline managed seamlessly through the CTO.ai developer platform.
* **Custom Habit Engine:** Dynamic, structured habit creation workflow with custom intervals.
* **Analytics Pipeline:** Backend calculations processing streak tracking alongside weekly & monthly progress trends.
* **Smart Reminders:** Cron-like alerting framework built natively into the application logic.
* **UX/UI Polish:** Fluid interface architecture featuring seamless dark mode support and structured daily reflection notes.

---

## DevOps & Pipeline Workflow (CTO.ai Integration)

Instead of relying on manual deployments or standard scripting hooks, Ripple utilizes **CTO.ai Pipelines and the CTO.ai SDK** to manage infrastructure as code:

1. **Local Dev to CLI:** Custom automated tasks configured via the SDK streamline local tracking and testing.
2. **Standardized Pipelines:** Automated workflows execute verification checks immediately upon code commits.
3. **Immutable Builds:** Code builds within isolated, reproducible containers to ensure zero drift between environments.
4. **Instant Production Sync:** Successful main-branch execution triggers automated deployment to live hosting.

---


---

##  Getting Started

### Prerequisites

- A [CTO.ai](https://cto.ai) account
- [Node.js](https://nodejs.org/) v16 or higher
- CTO.ai CLI installed

```bash
npm install -g @cto.ai/ops
```

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/sarajsair25/ripple-habit-tracker.git
cd ripple-habit-tracker
```

2. **Install dependencies**

```bash
npm install
```

3. **Authenticate with CTO.ai**

```bash
ops account:signin
```

4. **Run the app**

```bash
ops run .
```

---

##  Usage

Once the app is running, you'll be guided through an interactive CLI experience:

```
 Good morning! Ready to check in on your habits?

 Your habits for today:
  [ ]  Drink 8 glasses of water
  [ ]  30-minute workout
  [ ]  Read for 20 minutes
  [ ]  Meditate for 10 minutes

→ Select habits to mark as complete...
```

- Use **arrow keys** to navigate
- Press **Space** to toggle a habit complete
- Press **Enter** to save your check-in
- Type `ops run . --summary` to view your weekly progress report

---
##  Engineering Lessons Learned
Building Ripple from concept to a live deployment forced real-world engineering decisions:
* **System Automation over Manual Tasks:** Standardizing the delivery flow using a structured platform reduces deployment friction to zero.
* **Clean Code Separation:** Ensuring that application engine logic remains entirely separate from pipeline configuration hooks.
* **Product Accountability:** Developing features strictly against user-centric workflows rather than over-engineering complex technical logic.


##  Project Structure

```
ripple-habit-tracker/
├── ops.yml              # CTO.ai workflow configuration
├── src/
│   ├── index.js         # App entry point
│   ├── habits.js        # Habit CRUD logic
│   ├── tracker.js       # Check-in & streak logic
│   └── stats.js         # Progress & analytics
├── data/
│   └── habits.json      # Local habit store (auto-generated)
├── package.json
└── README.md
```

---

---

##  Roadmap

- [ ] Web dashboard with charts
- [ ] Habit sharing with friends
- [ ] Weekly email digest
- [ ] AI-powered habit suggestions
- [ ] Mobile push notifications
- [ ] Export data to CSV

---

##  Contributing

Contributions are welcome! Here's how to get started:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct.

---

##  License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

- Built with ❤️ on the [CTO.ai](https://cto.ai) platform
- Inspired by the philosophy of *Atomic Habits* by James Clear
- Name inspired by the idea that small actions create lasting ripples of change

---

## 📬 Connect

Have feedback or questions? Find me on:

- 💼 [LinkedIn](https://linkedin.com/sarahsair)
- **Email:** [sarahsair@gmail.com]


---

<p align="center">Made with ☕ and consistency · <strong>Ripple 🌊</strong></p>
