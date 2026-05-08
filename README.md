<h1 align="center">Hi, I'm Vikas Kumar</h1>
<p align="center">
  <b>Founding Engineer · Full-Stack · AI Systems</b>
</p>

<p align="center">
  <a href="https://helloviks.com"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/vikas-kumar45/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://medium.com/@imvk45"><img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"></a>
  <a href="mailto:kumav25@wfu.edu"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

### About

I build 0-to-1 AI products end to end. Frontend, backend, infra, evals, the design polish at the end. I care about shipping fast, making systems that hold up in production, and the small UX details that make AI tools feel human.

Currently an AI Engineer at Wake Forest University School of Business, founder of [SViam.in](https://sviam.in), and a Founding AI Engineer on MAP. Previously shipped a multilingual legal AI to 2,000+ users at Lawroom AI and a $3.2M annual savings optimization engine at Aditya Birla Group. Background in RLHF and red-teaming at Scale AI.

MS in Business Analytics at Wake Forest (4.0 GPA, fully funded), B.Tech in Data Science from Plaksha University (founding cohort, full merit scholarship).

---

### Projects

**[SViam.in](https://sviam.in)** — Two-way AI interview platform

A live AI interviewer that dynamically interrupts, probes, and adapts in real time, distinct from the pre-loaded question formats most platforms ship with. Candidates speak naturally, the system listens, decides when to push deeper, and grades reasoning across the conversation.

Built on Next.js 14 (App Router), React 19, TypeScript, Tailwind, and shadcn/ui on the frontend, with a FastAPI + Python 3.11 backend on Supabase Postgres + Storage. Real-time voice runs through ElevenLabs TTS and Deepgram STT (server-side REST), code interviews execute in sandboxed environments via the Piston API, and Monaco powers the in-browser code editor. Multi-agent orchestration is handled with Claude through OpenRouter.

The platform also runs a 5-stage resume tailoring engine (JD analyzer → matcher → selector → rewriter → verifier) anchored to verified user facts to prevent hallucination. Originally bottlenecked on sequential per-bullet inserts; now parallelized with asyncio and batch Postgres writes for end-to-end latency under target.

---

**[OmniPro Support](https://omnipro.helloviks.com/)** — Agentic multimodal voice assistant for industrial welding

Built for the Prox Founding Engineer Challenge. Shipped 14 production features in 49 hours, deployed live with a custom domain.

The product solves a real workflow problem: welders working on the Vulcan OmniPro 220 can't stop mid-arc to flip through a manual. OmniPro Support gives them a hands-free voice loop where they ask a question out loud and get an answer back in real time, all while their hands stay on the torch.

Reliability matters here because welding has real safety stakes, so every response runs through multi-agent deliberation. A Technical Specialist drafts the answer, a Safety Agent flags hazards, and a Quality Reviewer checks for completeness before the response goes out. Grounding is three layers deep: the official manual, troubleshooting guides, and a weld defect reference, all retrieved per query.

Beyond the voice loop, the system supports weld photo diagnosis (upload a photo of a bad weld, get root-cause analysis), machine photo annotation (point at the welder, get part identification), session-level memory across visits, an onboarding tour, and a customer mode toggle that switches between end-user and technician views.

Stack: Next.js 14, TypeScript, shadcn/ui, Tailwind, the Anthropic SDK with Claude Sonnet 4, ElevenLabs TTS, deployed on Vercel.

[Live Demo](https://omnipro.helloviks.com/) · [Repo](https://github.com/thisisvk45/prox-challenge)

---

**MAP (Music Advocacy Project)** — Concert ticket demand forecasting platform

Predicts fill rates for live music shows from artist signals, venue features, and external context. Users input artist + venue + date; the system pulls real-time social and artist data from Chartmetric, weather from OpenWeather, and merges with a static venue dataset.

The model layer runs a global XGBoost model with venue as a categorical feature plus venue mean fill rate as a numeric feature (the strongest single predictor at ~44% feature importance). On top of that, an ensemble system adds LLM predictions from Claude, Grok, and Mistral via OpenRouter, with smart resume from partial runs and row-by-row Excel saving for long-running pipelines.

Data work behind it: a Chartmetric + Visual Crossing enrichment pipeline over 3,835 historical shows and 48 features (March 2021 - January 2026), with chunked processing, retry-on-rate-limit, and a multi-query artist name resolution strategy.

---

**Facial Identity Persistence System** — Cross-session identity vectors for image generation

Research project aggregating ArcFace embeddings from 4-5 reference images into a 512-dim master identity vector via confidence-weighted fusion, with a persistent cross-session identity store. Runs as a Gradio demo on HF Spaces (Docker SDK, Python 3.10-slim, runtime model downloads). Built on InsightFace, ArcFace, and SDXL; forked from instantX-research/InstantID.

[Repo](https://github.com/thisisvk45/InstantID)

---

### Stack

**Frontend** Next.js 14 (App Router) · React 19 · TypeScript · Tailwind · shadcn/ui · Monaco · component-driven dev, performance, accessibility  
**Backend** Python · FastAPI · async pipelines · background workers · Postgres · Supabase · Prisma · object storage  
**AI & Agents** Claude (Anthropic SDK + OpenRouter) · LangChain · LlamaIndex · MCP · multi-agent orchestration · RAG · fine-tuning · prompt engineering  
**Voice & Multimodal** ElevenLabs TTS · Deepgram STT · real-time voice loops · vision input  
**ML** PyTorch · Hugging Face · scikit-learn · XGBoost · LightGBM · model evaluation · drift monitoring  
**Data** PostgreSQL · Snowflake · MongoDB · Neo4j · ChromaDB · Airflow · ETL pipelines  
**Infra & DevOps** AWS (Bedrock, SageMaker) · Docker · Vercel · GitHub Actions · Terraform · structured logs · tracing  
**Tooling** Claude Code CLI · Cursor · Wispr Flow · Playwright · PyTest · LaTeX

---

### How I work

Recon-first: read before writing, then make surgical changes instead of broad refactors. One step at a time with checkpoints. Heavy user of Claude Code CLI with Git worktrees and scoped subagents for parallel work. I write prompts as carefully as I write code.

---

### Reach me

[helloviks.com](https://helloviks.com) · [LinkedIn](https://www.linkedin.com/in/vikas-kumar45/) · [Medium](https://medium.com/@imvk45) · kumav25@wfu.edu
