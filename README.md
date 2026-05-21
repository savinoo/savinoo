# Lucas Lorenzo Savino

RAG & AI Agent Engineer. Python, retrieval pipelines, and multi-agent orchestration.

I build AI systems that answer from a company's own documents and stay grounded in them. My work is mostly RAG pipelines, retrieval quality, and multi-agent orchestration. I came into it from ML fundamentals, after seeing that companies usually need their LLMs connected to their own data, not retrained.

## What I work on

- Production RAG pipelines with citations and audit trails
- Document ingestion across mixed formats such as PDF, DOCX, and spreadsheets
- Retrieval evaluation (recall@k, MRR) and hallucination control
- Multi-agent orchestration with LangGraph
- Agent infrastructure over the MCP protocol

## Featured projects

**[RAG Knowledge Base](https://github.com/savinoo/rag-knowledge-base)**
A RAG system for internal knowledge bases such as SOPs and policies. Every answer carries source citations, and a confidence threshold returns a "Not in KB yet" response instead of guessing. It includes a full audit trail and a built-in recall@k evaluation. Built with LangChain, ChromaDB, OpenAI, and Streamlit.

**[RAG Agent](https://github.com/savinoo/RAG_Agent)**
A stateful agentic RAG system on LangGraph. The agent decides whether retrieval is needed before answering and keeps conversation state across turns. PDF ingestion, chunking, and indexing are built in. Built with LangGraph, LangChain, ChromaDB, and OpenAI.

**[RAG Eval Harness](https://github.com/savinoo/rag-eval-harness)**
A small, reproducible evaluation harness for RAG. It runs a golden dataset, computes recall@k and MRR, and produces a shareable report. It is meant as a regression test to run before and after retrieval changes. Vector-database agnostic, with CI included.

**[AI Grading System](https://github.com/savinoo/ai-grading-system)**
My capstone project. A multi-agent system for grading discursive exam answers. Two grader agents evaluate each answer in parallel against a rubric and RAG-retrieved course material. A third arbiter agent runs only when their scores diverge beyond a threshold. In a controlled study it completed the full flow without failures, and RAG measurably improved evaluative specificity on intermediate-quality answers. Built with LangGraph, LangChain, FastAPI, ChromaDB, and PostgreSQL.

**[Daily Ops Agent](https://github.com/savinoo/daily-ops-agent)**
An autonomous agent that aggregates e-commerce operations metrics, detects anomalies against rolling baselines, and generates a prioritized daily action brief. Built with a clean adapter pattern and decision memory. Uses FastAPI, SQLite, and Docker.

**[Agentbridge](https://github.com/savinoo/agentbridge)**
A cross-IDE agent workflow orchestrator built on the MCP protocol. Workflows are defined in YAML, with each step assigned to a specific agent and dependency resolution between steps. Built with TypeScript, MCP, and SQLite.

## Tech

Python, LangChain, LangGraph, RAG, multi-agent systems, OpenAI API, ChromaDB. FastAPI, TypeScript, Node.js, PostgreSQL, SQLite, Docker. MCP (Model Context Protocol).

## Experience

**Petrobras**, AI Engineer Intern (2024 to 2026)
Built AJUDEM, an internal RAG assistant for the logistics area. It retrieves precedents from over 100 validated historical cases and past meeting minutes to support a recurring review process, and proposes a scored assessment with reasoning that a human confirms. It cut per-case review time from several minutes to around 20 seconds.

**Instituto Federal Fluminense**, BSc in Computer Engineering (2026)

## Contact

Open to freelance work on RAG systems, AI agents, and AI automation. Based in Brazil (GMT-3), working remotely and comfortable with US and EU hours.

Connect on [LinkedIn](https://linkedin.com/in/savinoo).
