🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎉 Soc Ops

**A social bingo icebreaker and hands-on GitHub Copilot Agent Lab.**

Soc Ops turns an in-person mixer into a lightweight game: players meet people, match friendly prompts, mark a 5×5 board, and race to get five in a row. The repo also doubles as a workshop for practicing agentic development with VS Code, GitHub Copilot, Java 21, and Spring Boot.

[📚 Start the Lab](workshop/GUIDE.md) · [🧭 View Overview](workshop/00-overview.md) · [🤝 Contribute](CONTRIBUTING.md)

---

## ✨ Why this project?

- **Instant icebreaker** — low-stakes prompts help people start conversations quickly.
- **Workshop ready** — follow a guided lab to explore context engineering, frontend iteration, custom agents, and TDD workflows.
- **Small, hackable stack** — Java 21, Spring Boot, Thymeleaf, plain JavaScript, and simple CSS utilities.
- **Agent-friendly codebase** — clear project instructions, custom agents, and focused exercises make it easy to experiment safely.

---

## 🕹️ What you can build

| Area | Try this |
|------|----------|
| Game experience | Refresh boards, tune prompts, and polish the bingo flow. |
| Frontend design | Redesign the page with a stronger visual theme and responsive layout. |
| Agent workflows | Create focused agents for quiz writing, cloud planning, UI review, or TDD. |
| Java logic | Extend board assembly, cell flipping, and winning-streak detection with tests. |

---

## 🚀 Quick start

### Prerequisites

- [Java 21 JDK](https://adoptium.net/) or higher
- [Apache Maven 3.9+](https://maven.apache.org/) or the included Maven Wrapper

### Run locally

```bash
cd socops
./mvnw spring-boot:run
```

Then open the local Spring Boot app in your browser.

### Build

```bash
cd socops
./mvnw clean package
```

### Test

```bash
cd socops
./mvnw test
```

> On Windows PowerShell, use `./mvnw.cmd` if `./mvnw` is not executable.

---

## 📚 Lab guide

| Part | Title | Focus |
|------|-------|-------|
| [**00**](workshop/00-overview.md) | Overview & Checklist | Get oriented and verify your environment. |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering | Teach the AI how this project works. |
| [**02**](workshop/02-design.md) | Design-First Frontend | Iterate on a more memorable game UI. |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master | Generate inclusive prompt themes with a custom agent. |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development | Combine agents for planning, TDD, and review. |
| [**05**](workshop/05-complete.md) | Complete | Wrap up and explore next steps. |

> 📝 Lab guides are also available in the [workshop/](workshop/) folder for offline reading.

---

## 🧩 Project map

```text
socops/                 Spring Boot application
	src/main/java/        Java domain, service, and web code
	src/main/resources/   Thymeleaf template and static CSS
	src/test/java/        JUnit tests
workshop/               Step-by-step lab materials
docs/                   GitHub Pages workshop site
.github/agents/         Custom Copilot agents for lab workflows
```

---

## 🤝 Contributing

Contributions are welcome. Start with [CONTRIBUTING.md](CONTRIBUTING.md), keep prompts inclusive and low-stakes, and add tests for Java behavior changes.

Deploys automatically to GitHub Pages on push to `main`.
