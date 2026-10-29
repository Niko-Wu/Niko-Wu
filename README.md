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

### [testcase-kb](https://github.com/Niko-Wu/testcase-kb) — an executable test-case knowledge base

A local-first Claude Code plugin that treats test cases as team knowledge: describe a case in one sentence, get a runnable test.

- **Dual-source by construction** — every case is a design doc (markdown) plus a Playwright spec, assertions isomorphic between the two; selectors are probe-verified against the real page, never guessed
- **Zero-AI execution** — cases compile to pure Playwright specs that run headless in CI; verdicts come only from spec assertions
- **Share by link, not by install** — a local site serves progress, failure evidence and screenshots to teammates on the LAN
- **Private by default** — data lives in `~/.testcase-kb`; teams wanting a shared library just push the data dir, it's all markdown

### Typed judgments for agents (research)

Exploring [TypeSafe](https://typesafe.ai)'s System One models — **[Jev](https://docs.typesafe.ai)**, its flagship model that turns natural language into typed, composable judgments — as a primitive for agent routing, ranking and verification inside these workflows.

## 🔁 Open Source

Contributing to **[chenhg5/cc-connect](https://github.com/chenhg5/cc-connect)** (15k+ ⭐) — bridging IM platforms to local coding agents.

**Merged**

- [#1709](https://github.com/chenhg5/cc-connect/pull/1709) `feat(cursor)` — deliver image attachments to the Cursor CLI via on-disk paths, with MIME-based extension inference
- [#1710](https://github.com/chenhg5/cc-connect/pull/1710) `fix(daemon)` — drop redundant `CheckLinger` stub that broke all non-Linux builds
- [#1738](https://github.com/chenhg5/cc-connect/pull/1738) `fix(pi)` — remove unused `os` import that broke Windows builds
- [#1926](https://github.com/chenhg5/cc-connect/pull/1926) `fix(core)` — derive the workspace session store from the engine store path

**Approved, awaiting merge**

- [#1778](https://github.com/chenhg5/cc-connect/pull/1778) `feat(feishu)` — AskUserQuestion card 2.0: option buttons + free-form input, with one-time session-bound tokens, server-side answer validation and full i18n
- [#1757](https://github.com/chenhg5/cc-connect/pull/1757) `fix(core)` — trailing `NO_REPLY` must not suppress text already delivered before a tool call
- [#1755](https://github.com/chenhg5/cc-connect/pull/1755) `fix(claudecode)` — add `claude-fable-5` to the `/model` fallback list
- [#1925](https://github.com/chenhg5/cc-connect/pull/1925) `chore` — gofmt the tree

**In review**

- [#1756](https://github.com/chenhg5/cc-connect/pull/1756) `fix(daemon)` — set `HOME` in systemd system units so the default `data_dir` resolves
- [#1754](https://github.com/chenhg5/cc-connect/pull/1754) `fix(preset)` — correct the Kimi API registration link

Also contributing to **[yetone/magpie](https://github.com/yetone/magpie)** — a fix that landed via cherry-pick: [#2219](https://github.com/yetone/magpie/issues/2219) replaces a wall-clock bound in a big-TOML parse test with a size-ratio check, so a loaded runner no longer produces a false red. Cherry-picked as `36200091a`, with the maintainer widening it in `99299c7b1`; listed in the repository's contributors.

And to **[rtk-ai/rtk](https://github.com/rtk-ai/rtk)** — [#3709](https://github.com/rtk-ai/rtk/pull/3709) `fix(stream)`: report a signal-terminated child instead of silently exiting with `128 + signal`.

I also build daily on top of open agent tooling — [spec-kit](https://github.com/github/spec-kit), [Claude Code](https://github.com/anthropics/claude-code), and the agent-CLI ecosystem around them.

## 📬 Contact

<p align="center">
  <img alt="WeChat" src="https://img.shields.io/badge/WeChat-From__0714-07C160?style=flat-square&logo=wechat&logoColor=white">
</p>

<p align="center">Always happy to talk about agents, open source, or anything in between.</p>

<p align="center"><sub>Email and location are in the sidebar — or just open an issue / discussion on a repo I'm active in.</sub></p>
