# Lucas Lorenzo Savino

**AI Engineer — agents, context engineering, RAG with a human in the loop**

I design the system around the model, not the prompt. The decisions that matter are
which documents enter the context window, when an extra agent is worth its cost,
what the model is deliberately *not* allowed to see, and where a person confirms
before a decision counts.

Computer Engineering, Instituto Federal Fluminense (2026). Almost two years at
Petrobras, in logistics, putting an LLM inside a real decision process.

## What I decide when I build these systems

- **Context scoping** — what enters the window, what stays out, and why leakage between cases invalidates the output and the experiment measuring it
- **Agent topology** — isolated context so parallel agents don't anchor on each other; conditional routing so the expensive agent only runs when it earns its place
- **Human confirmation** — the system proposes with reasoning and sources; a person approves before the result is authoritative, and every decision stays traceable to the criterion behind it
- **Honest evaluation** — measuring whether retrieval actually helped, and reporting the cases where it changed nothing
- **AWS serverless when the thing has to actually run** — Lambda, S3, DynamoDB, Cognito, SQS, CDK

## Projects

### [ai-grading-system](https://github.com/savinoo/ai-grading-system) — capstone (TCC)

Multi-agent grading of discursive exam answers, modelled on the ENEM process of two
independent graders plus a referee.

Two examiners score the same answer in **isolated context** — neither sees the other's
score or reasoning — and a third agent is invoked **only** when their divergence crosses
a threshold. RAG is hard-scoped per exam with no global fallback, because context leaking
between exams would contaminate both the grading and the study measuring it.

Controlled study, 24 graded answers. RAG improved evaluative specificity on mid-range
answers (Δ = +0.84) and changed nothing at the extremes. The referee never fired: real
divergence peaked at 1.22 against a threshold of 2.0, which says the threshold needed
empirical calibration rather than a guess. Weak answers failed the stability criterion.
Both negative results are in the README, along with what I would do differently.

`LangGraph` · `LangChain` · `FastAPI` · `ChromaDB` · `PostgreSQL`

### Portal da Produtora — iOS + AWS serverless *(private repo)*

Media ingestion and review platform for a video production studio, replacing ad-hoc
file sending with a traceable flow. Native iPhone app, web review portal, serverless
backend. Deployed to AWS and validated on a real device.

The design constraint that shaped everything: **upload and publication are independent
operations** — putting a file in the cloud never exposes it to the client. Multipart
uploads go straight from the phone to S3 through pre-signed URLs in resumable 16 MiB
parts, so the file never travels through the API. Derivation runs async behind SQS with
a dead-letter queue and idempotent Lambdas, so a retry can't duplicate an upload.

42 backend tests, 35 native iOS tests, infrastructure validated by CDK synth.

`Swift` · `TypeScript` · `CDK` · `Lambda ARM64` · `DynamoDB` · `S3` · `Cognito (OAuth 2.0 + PKCE)` · `SQS` · `MediaConvert` · `CloudFront`

### AJUDEM — Petrobras, logistics *(internal, not public)*

Monthly audit of stock-discrepancy justifications submitted by a partner company. The
coordinator read each justification and accepted or rewrote it by hand; closing the
indicator took hours.

I started with a syntactic adherence indicator between the submitted text and the
coordinator's corrected version. The RAG stage came later, once it was clear that the
history of accepts and rejects was the context that was missing: the system retrieves
precedents from 100+ validated cases and meeting minutes, proposes a 0–10 score with its
reasoning, and an analyst confirms before the decision enters the corpus.

Time spent on that indicator fell from **~3 hours/week on average to at most 2–10 minutes**.

It only became part of the routine once the team trusted the output enough to bring it
into a live negotiation meeting. That took sitting with the analysts to find where their
bar was stricter than the code's — not tuning the prompt.

## Also in this account

Coursework and experiments from earlier on, kept because they're part of the record:
[PCA implementation](https://github.com/savinoo/PCA-implementation),
[a neural network that drives a car](https://github.com/savinoo/self-driving-car-with-neural-network).
They are what they look like — things I built while learning.

## Now

Open to **AI engineering / agent engineering** roles, in Python. Remote, or hybrid and
on-site in Rio de Janeiro.

Studying for the AWS Solutions Architect Associate, exam booked for September 2026.

[LinkedIn](https://linkedin.com/in/savinoo)
