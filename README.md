<div align="center">

# Vikas Kumar

### AI Engineer · Voice AI · RAG · Production ML

*I take AI systems from an empty repo to real users: frontend, backend, infra, evals,*  
*and the small UX details that make AI tools feel human.*

<br>

[![Portfolio](https://img.shields.io/badge/helloviks.com-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://helloviks.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vikas-kumar45/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@imvk45)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:meet.kumarvikas@gmail.com)

</div>

---

## Currently

```text
~ Founding Full-Stack Engineer  @ The M.A.P. (Music Advocacy Project)   May 2026 - present

Previously
~ AI Engineer                   @ Wake Forest School of Business         RAG for 500+ students, 40+ advisors
~ Founder & AI Engineer         @ SViam                                  Maya, a real-time voice interviewer
~ Founding Full-Stack Engineer  @ Lawroom AI                             0 to 6,000+ users
~ AI/Software Engineer Intern   @ Aditya Birla Group                     $3.2M annual savings
~ RLHF / Red-Teaming            @ Scale AI
```

---

## The M.A.P.: ticket-demand forecasting for live music

Predicts ticket sales for shows so venues and promoters can book with confidence. I built the platform end to end (React frontend, Python backend, data pipelines, model serving, deployment) and the model behind it.

```text
Model     →  CatBoost plus LLM reasoning over artist tiers, venue history, social signals, local competition
Scale     →  15,814 events · 150+ venues
Result    →  74% accuracy, ahead of Claude, GPT and Grok on the same forecasts
```

Most of the real work happens outside the model: sitting with venue operators, watching where predictions break, and shipping fixes to partners on deadline. (Private repo.)

---

## Things I've built

### [OmniPro Support](https://omnipro.helloviks.com/): multimodal voice agent for industrial welding

Built for the Prox (YC F25) Founding Engineer Challenge. **14 production features in 49 hours.** Live with a custom domain.

Welders working on the Vulcan OmniPro 220 cannot stop mid-arc to flip through a manual. OmniPro Support gives them a hands-free voice loop: they ask out loud and get an answer back in real time, hands stay on the torch.

Welding has real safety stakes, so every response runs through multi-agent deliberation:

```text
Technical Specialist  →  drafts the answer
Safety Agent          →  flags hazards
Quality Reviewer      →  checks for completeness
```

Grounding is three layers deep (official manual, troubleshooting guides, weld defect reference), retrieved per query. Also: weld photo diagnosis, machine photo annotation, session memory across visits, and a customer mode toggle for end-user vs. technician views.

```text
Stack  →  Next.js 14 · TypeScript · shadcn/ui · Tailwind · Anthropic SDK · ElevenLabs · Vercel
```

[Live Demo](https://omnipro.helloviks.com/) · [Repo](https://github.com/thisisvk45/prox-challenge)

---

### Maya: real-time voice interviewer (SViam, Jun 2025 to May 2026)

A voice agent that runs full coding interviews over WebRTC and drives the live UI through 31 client tools: code editing, highlighting, algorithm walkthroughs, and automated reports. It interrupts, probes, and adapts instead of reading from a fixed question list.

Two models with separate contexts: a conversation model that sees the last few turns and replies fast, and a judge model that sees the whole session and grades against a rubric.

```text
Frontend  →  Next.js · React · TypeScript · Monaco · Pyodide
Backend   →  FastAPI · Supabase · Redis
Voice     →  LiveKit · ElevenLabs
Infra     →  AWS Amplify · ECS Fargate · CloudFront
```

---

### [JobForge](https://github.com/thisisvk45/Jobforge): autonomous job search pipeline

Pulls roles from Greenhouse, Lever and Ashby, pre-filters with Claude Haiku, evaluates with Sonnet, runs RAG over a personal corpus in ChromaDB, and drafts tailored CVs and cover letters. 97/97 tests passing.

---

### [Facial Identity Persistence System](https://github.com/thisisvk45/InstantID): cross-session identity vectors

Aggregates ArcFace embeddings from 4-5 reference images into a **512-dim master identity vector** via confidence-weighted fusion, with a persistent cross-session identity store. Gradio demo on HF Spaces. Built on InsightFace, ArcFace and SDXL; forked from instantX-research/InstantID.

---

## Stack

```text
Frontend     Next.js · React · TypeScript · Tailwind · shadcn/ui · Monaco
Backend      Python · FastAPI · async pipelines · workers · Postgres · Supabase · Prisma · Redis
AI / Agents  Claude · OpenRouter · LangChain · LlamaIndex · MCP · RAG · evals · fine-tuning
Voice        LiveKit · ElevenLabs · Deepgram · WebRTC · real-time voice loops
ML           PyTorch · HuggingFace · CatBoost · XGBoost · LightGBM · drift monitoring
Data         PostgreSQL · Snowflake · MongoDB · Neo4j · ChromaDB · Airflow
Infra        AWS · Docker · Vercel · GitHub Actions · Terraform · structured logs
Tooling      Claude Code CLI · Cursor · Wispr Flow · Playwright · PyTest · LaTeX
```

---

## How I work

Recon first: read before writing, then make surgical changes instead of broad refactors. One step at a time with checkpoints. Heavy user of Claude Code with git worktrees and scoped subagents for parallel work. I write prompts as carefully as I write code, and I build the eval before I scale the system.

---

<div align="center">

[helloviks.com](https://helloviks.com) · [LinkedIn](https://www.linkedin.com/in/vikas-kumar45/) · [Medium](https://medium.com/@imvk45) · meet.kumarvikas@gmail.com

</div>
