<h1 align="center">Hi, I'm Niko 👋</h1>

<p align="center">
  <b>Agent Engineer @ Tuya</b> — building multi-agent developer workflows:<br>
  <sub>agent orchestration · spec-driven development pipelines · agent design on coding-agent runtimes</sub>
</p>

<p align="center">
  <img alt="Claude Code" src="https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white">
  <img alt="Go" src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white">
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white">
  <img alt="Spring" src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
</p>

## ⚡ What I'm building

### speckit-workflow — a spec-driven, multi-agent development pipeline

A Claude Code plugin I designed and built at Tuya, in daily use on our team. It takes a feature from a one-line request to deployed code, end to end:

- **One pipeline, seven stages** — `specify → grill → plan → validate → sync → implement → test`, advanced by a router that reads a per-workspace `pipeline.yaml`
- **A five-role agent team** — software architect (lead) / backend architect / frontend developer / functional tester / DevOps automator, each stage dispatching to the right role and model tier
- **19 skills** — Socratic PRD decomposition into acceptance criteria, technical design with e2e-spec derivation, pre-code quality gates, multi-repo parallel coding with compile + LSP + unit-test gates, and a test stage that drives a fix-loop to green
- **Deterministic hooks** — objective, file-level checks run as scripts the model cannot skip; judgment calls stay with an LLM reviewer
- **Knowledge that compounds** — each finished project is curated into an Obsidian wiki (project / app / concept pages), so past decisions and pitfalls feed the next design

### Typed judgments for agents (research)

Exploring [TypeSafe](https://typesafe.ai)'s System One models — **[Jev](https://docs.typesafe.ai)**, its flagship model that turns natural language into typed, composable judgments — as a primitive for agent routing, ranking and verification inside these workflows.

## 🔁 Open Source

Contributing to **[chenhg5/cc-connect](https://github.com/chenhg5/cc-connect)** (15k+ ⭐) — bridging IM platforms to local coding agents.

**Merged**

- [#1709](https://github.com/chenhg5/cc-connect/pull/1709) `feat(cursor)` — deliver image attachments to the Cursor CLI via on-disk paths, with MIME-based extension inference
- [#1710](https://github.com/chenhg5/cc-connect/pull/1710) `fix(daemon)` — drop redundant `CheckLinger` stub that broke all non-Linux builds
- [#1738](https://github.com/chenhg5/cc-connect/pull/1738) `fix(pi)` — remove unused `os` import that broke Windows builds

**Approved, awaiting merge**

- [#1778](https://github.com/chenhg5/cc-connect/pull/1778) `feat(feishu)` — AskUserQuestion card 2.0: option buttons + free-form input
- [#1757](https://github.com/chenhg5/cc-connect/pull/1757) `fix(core)` — trailing `NO_REPLY` must not suppress text already delivered before a tool call
- [#1755](https://github.com/chenhg5/cc-connect/pull/1755) `fix(claudecode)` — add `claude-fable-5` to the `/model` fallback list

I also build daily on top of open agent tooling — [spec-kit](https://github.com/github/spec-kit), [Claude Code](https://github.com/anthropics/claude-code), and the agent-CLI ecosystem around them.

## 📬 Contact

<p align="center">
  <img alt="WeChat" src="https://img.shields.io/badge/WeChat-From__0714-07C160?style=flat-square&logo=wechat&logoColor=white">
</p>

<p align="center">Always happy to talk about agents, open source, or anything in between.</p>

<p align="center"><sub>Email and location are in the sidebar — or just open an issue / discussion on a repo I'm active in.</sub></p>
