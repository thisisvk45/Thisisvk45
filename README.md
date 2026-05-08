<div align="center">

# Vikas Kumar

### Founding Engineer · Full-Stack · AI Systems

*I build 0-to-1 AI products end to end. Frontend, backend, infra, evals,*  
*and the small UX details that make AI tools feel human.*

<br>

[![Portfolio](https://img.shields.io/badge/helloviks.com-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://helloviks.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vikas-kumar45/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@imvk45)
[![Email](https://img.shields.io/badge/kumav25@wfu.edu-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kumav25@wfu.edu)

</div>

---

## Currently

```text
~ AI Engineer        @ Wake Forest School of Business
~ Founder            @ SViam.in
~ Founding Engineer  @ MAP (Music Advocacy Project)

Previously
~ Founding AI Engineer  @ Lawroom AI         (scaled to 2,000+ users)
~ ML Engineer Intern    @ Aditya Birla Group ($3.2M annual savings)
~ RLHF / Red-Teaming    @ Scale AI
```

---

## Things I'm building

### [SViam.in](https://sviam.in) — Two-way AI interview platform

A live AI interviewer that dynamically interrupts, probes, and adapts in real time. Distinct from the pre-loaded question formats most platforms ship with. Candidates speak naturally, the system listens, decides when to push deeper, and grades reasoning across the conversation.

```text
Frontend  →  Next.js 14 · React 19 · TypeScript · Tailwind · shadcn/ui · Monaco
Backend   →  FastAPI · Python 3.11 · Supabase Postgres + Storage
Voice     →  ElevenLabs TTS · Deepgram STT
Compute   →  Piston API (sandboxed code execution)
Agents    →  Claude via OpenRouter, multi-agent orchestration
```

Also runs a 5-stage resume tailoring engine: **JD analyzer → matcher → selector → rewriter → verifier**, anchored to verified user facts to prevent hallucination. Parallelized with asyncio and batch Postgres writes for low end-to-end latency.

---

### [OmniPro Support](https://omnipro.helloviks.com/) — Multimodal voice agent for industrial welding

Built for the Prox Founding Engineer Challenge. **14 production features in 49 hours.** Live with a custom domain.

The product solves a real workflow problem: welders working on the Vulcan OmniPro 220 cannot stop mid-arc to flip through a manual. OmniPro Support gives them a hands-free voice loop where they ask out loud and get an answer back in real time, hands stay on the torch.

Reliability matters because welding has real safety stakes, so every response runs through multi-agent deliberation:

```text
Technical Specialist  →  drafts the answer
Safety Agent          →  flags hazards
Quality Reviewer      →  checks for completeness
```

Grounding is three layers deep (official manual, troubleshooting guides, weld defect reference), retrieved per query.

Beyond the voice loop: weld photo diagnosis, machine photo annotation, session-level memory across visits, an onboarding tour, and a customer mode toggle for end-user vs. technician views.

```text
Stack  →  Next.js 14 · TypeScript · shadcn/ui · Tailwind · Anthropic SDK (Claude Sonnet 4) · ElevenLabs · Vercel
```

[Live Demo](https://omnipro.helloviks.com/) · [Repo](https://github.com/thisisvk45/prox-challenge)

---

### MAP (Music Advocacy Project) — Concert ticket demand forecasting

Predicts fill rates for live music shows from artist signals, venue features, and external context. User inputs artist + venue + date; system pulls real-time data and predicts.

```text
Signals  →  Chartmetric (artist + social) · OpenWeather · static venue dataset
Model    →  Global XGBoost (venue as categorical, venue mean fill rate as numeric)
Ensemble →  Claude + Grok + Mistral predictions via OpenRouter
Pipeline →  Smart resume from partial runs · row-by-row Excel saving
```

Behind it: a Chartmetric + Visual Crossing enrichment pipeline over 3,835 shows and 48 features (Mar 2021 — Jan 2026), with chunked processing, retry-on-rate-limit, and a multi-query artist name resolution strategy. Venue mean fill rate dominated feature importance at ~44%; SML/capacity ratio was the strongest single predictor.

---

### [Facial Identity Persistence System](https://github.com/thisisvk45/InstantID) — Cross-session identity vectors

Aggregates ArcFace embeddings from 4-5 reference images into a **512-dim master identity vector** via confidence-weighted fusion, with a persistent cross-session identity store. Runs as a Gradio demo on HF Spaces (Docker SDK, Python 3.10-slim). Built on InsightFace, ArcFace, and SDXL; forked from instantX-research/InstantID.

---

## Stack

```text
Frontend     Next.js · React · TypeScript · Tailwind · shadcn/ui · Monaco
Backend      Python · FastAPI · async pipelines · workers · Postgres · Supabase · Prisma
AI / Agents  Claude · OpenRouter · LangChain · LlamaIndex · MCP · RAG · fine-tuning
Voice        ElevenLabs · Deepgram · real-time voice loops
ML           PyTorch · HuggingFace · XGBoost · LightGBM · drift monitoring
Data         PostgreSQL · Snowflake · MongoDB · Neo4j · ChromaDB · Airflow
Infra        AWS · Docker · Vercel · GitHub Actions · Terraform · structured logs
Tooling      Claude Code CLI · Cursor · Wispr Flow · Playwright · PyTest · LaTeX
```

---

## How I work

Recon-first: read before writing, then make surgical changes instead of broad refactors. One step at a time with checkpoints. Heavy user of Claude Code CLI with Git worktrees and scoped subagents for parallel work. I write prompts as carefully as I write code.

---

<div align="center">

[helloviks.com](https://helloviks.com) · [LinkedIn](https://www.linkedin.com/in/vikas-kumar45/) · [Medium](https://medium.com/@imvk45) · kumav25@wfu.edu

</div>
