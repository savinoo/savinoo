# Lucas Lorenzo Savino

**AI Agent Engineer** | Multi-Agent Systems, RAG & LLM Orchestration

Building autonomous AI systems that work in production — not just demos.

---

## 🎯 What I Do

I specialize in **AI agent development** and **multi-agent orchestration**. The kind of systems where an AI doesn't just chat — it reasons, retrieves verified information, collaborates with other agents, and takes action autonomously.

**Current Focus:**
- Multi-agent systems with LangGraph + DSPy
- Production RAG pipelines with citations & audit trails
- Agent orchestration infrastructure (MCP protocol)
- Business automation with AI agents

---

## 🚀 Featured Projects

### [AI Grading System](https://github.com/savinoo/ai-grading-system) — Multi-Agent Academic Assessment
**The flagship project.** Three AI agents (2 Examiners + 1 Arbiter) grade complex essay questions autonomously. When agents disagree beyond a threshold, the Arbiter reviews both arguments and makes the final call — mirroring real academic committees.

- **Results:** 5x throughput improvement, 90% fewer DB queries via intelligent caching
- **Tech:** LangGraph, DSPy, LangChain, ChromaDB, Streamlit
- **Status:** In pilot with professors at Instituto Federal Fluminense

### [Agentbridge](https://github.com/savinoo/agentbridge) — Cross-IDE Agent Workflow Orchestrator
In 2026, teams use multiple AI coding agents (Claude Code, Antigravity, Cursor) — but they don't talk to each other. **Agentbridge solves this.**

Define workflows in YAML. Each step is assigned to a specific agent. When one finishes, the next unblocks automatically. Dependency resolution, conditional execution, cross-agent handoff — all handled.

- **Verified E2E** with 2 simulated agents via HTTP sessions
- **Tech:** TypeScript, MCP (Model Context Protocol), SQLite, YAML
- **Differentiator:** One of the first MCP orchestrators on GitHub

### [Daily Ops Agent](https://github.com/savinoo/daily-ops-agent) — E-commerce Intelligence Brief Generator
Autonomous AI agent that aggregates metrics from Shopify, Meta Ads, and Google Ads, detects anomalies against rolling baselines, and generates prioritized action items daily.

- **What it solves:** Reduces 45-60 min/day of manual dashboard checking to seconds
- **Tech:** FastAPI, SQLite, Docker, Jinja2 templating
- **Architecture:** Clean adapter pattern, decision memory, one-click Render deploy

### [WhatsApp Agentic Daemon](https://github.com/savinoo/whatsapp-mcp) — AI Agent via WhatsApp
Turn WhatsApp into a full agentic interface. Send a message from your phone, Claude executes on your Mac with full tool access, and sends back the result — including modified files.

- **Features:** Streaming with heartbeat, session continuity, auto file sharing, cost tracking, 8 slash commands
- **Tech:** Python, Claude CLI (stream-json), SQLite, Go (WhatsApp bridge)
- **Architecture:** Webhook daemon + Go bridge + Claude CLI with process management

### [RAG Knowledge Base System](https://github.com/savinoo/simple-rag-chatbot) — Grounded Q&A with Citations
Enterprise-ready RAG system with mandatory citations, confidence thresholds ("Not in KB yet" fallback), full audit trail (JSONL + SQLite), and built-in retrieval evaluation harness.

- **Tech:** LangChain, ChromaDB, OpenAI/Gemini, Streamlit
- **Features:** Manifest-driven ingestion, recall@k metrics, section-level citations

---

## 🛠️ Tech Stack

**AI/ML:**
`Python` `LangChain` `LangGraph` `DSPy` `OpenAI API` `Anthropic Claude` `ChromaDB` `RAG` `Multi-Agent Systems`

**Backend & Infra:**
`FastAPI` `TypeScript` `Node.js` `SQLite` `Docker` `Git` `CI/CD`

**Agent Orchestration:**
`MCP (Model Context Protocol)` `State Machines` `Workflow Engines`

---

## 📈 The Journey (4 Acts)

**Act 1 — Foundations (2023-2024)**
Started with ML fundamentals: implemented PCA from scratch, built neural networks for self-driving car simulation. Understood the math before jumping to LLMs.

**Act 2 — RAG Mastery (2025)**
Dove deep into RAG when I realized most businesses don't need to train models — they need to connect LLMs to their own data. Built stateful RAG systems with LangGraph that decide autonomously when to retrieve.

**Act 3 — Multi-Agent Systems (2025-2026)**
Evolved from simple agents to **multi-agent orchestration**. In my capstone project (TCC), built a 3-agent grading system — the same pattern used by Anthropic and Google for complex reasoning tasks.

**Act 4 — Agent Infrastructure (2026)**
Now working on the infrastructure layer: how to orchestrate workflows across agents from different platforms. Created Agentbridge, a cross-IDE orchestrator using the MCP protocol.

---

## 💼 Experience

**Petrobras** — AI/ML Engineering Intern
Working on AI/ML projects at Brazil's largest company (Fortune 500)

**Instituto Federal Fluminense** — Computer Engineering
Graduating April 2026

---

## 📫 Let's Work Together

🔹 **Open to freelance projects:** AI agent development, RAG systems, multi-agent workflows, AI automation
🔹 **Location:** Brazil (GMT-3) | Remote-friendly | US/EU hours available
🔹 **Rate:** $60-80/hr (mid-level specialist)

📧 Contact me for: AI agent development • RAG pipelines • Multi-agent systems • Business automation

---

<div align="center">

[![GitHub followers](https://img.shields.io/github/followers/savinoo?style=social)](https://github.com/savinoo)
[![GitHub stars](https://img.shields.io/github/stars/savinoo?style=social)](https://github.com/savinoo)

*Building the future of autonomous AI, one agent at a time* 🤖

</div>
