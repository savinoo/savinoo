# Lucas Lorenzo Savino

Applied AI Engineer | RAG, agents, and LLM evaluation | Ex-Petrobras

I build systems that score and retrieve against a company's own documents, with citations, an audit trail, and a human in the loop. The recurring problem is not generating text. It is knowing whether the output is grounded.

## What I work on

- RAG pipelines with source citations and a fallback when retrieval is weak
- Retrieval evaluation (recall@k, MRR) before and after indexing changes
- Multi-agent scoring: independent graders plus a conditional arbiter
- Document ingestion across PDF, DOCX, and spreadsheets
- AWS serverless when the system has to run (Lambda, S3, DynamoDB, Cognito, CDK)

## Featured projects

**[AI Grading System](https://github.com/savinoo/ai-grading-system)** — capstone (TCC)
Two examiner agents grade a discursive answer in parallel against a rubric and RAG-retrieved course material. A third arbiter runs only when their scores diverge. Controlled study: 24 graded answers, full end-to-end completion, RAG improved evaluative specificity on intermediate-quality answers (Δ = +0.84). LangGraph, FastAPI, ChromaDB, PostgreSQL.

**[RAG Eval Harness](https://github.com/savinoo/rag-eval-harness)**
Regression test for retrieval. Golden dataset, recall@k, MRR, shareable report. Vector-store agnostic, CI included.

**[RAG Knowledge Base](https://github.com/savinoo/rag-knowledge-base)**
Internal SOP/policy assistant. Every answer cites sources. Below a confidence threshold it answers "Not in KB yet" instead of guessing. Audit log plus built-in recall@k.

**[RAG Agent](https://github.com/savinoo/RAG_Agent)**
Stateful agentic RAG on LangGraph. The agent decides whether retrieval is needed, then keeps conversation state across turns.

## Experience

**Petrobras** — Computer Engineering intern, Logistics (2024–2026)

Built AJUDEM, an internal RAG assistant for a recurring review process. It retrieves precedents from 100+ validated historical cases and meeting minutes, proposes a 0–10 score with reasoning, and a human confirms before the decision enters the corpus. In a monthly pilot, per-case review fell from several minutes to about 20 seconds; unresolved monthly items fell from 10–15 to fewer than 3.

**Instituto Federal Fluminense** — BSc Computer Engineering (2026)

## Contact

Open to full-time roles in applied AI, data/analytics engineering, and Python backend. Rio de Janeiro or remote.

[LinkedIn](https://linkedin.com/in/savinoo) · [ai-grading-system](https://github.com/savinoo/ai-grading-system) · [rag-eval-harness](https://github.com/savinoo/rag-eval-harness)
