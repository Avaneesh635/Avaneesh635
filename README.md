<h1 align="center">Hi , I'm Avaneesh Joshi</h1>
<h3 align="center">AI/ML Engineer | GenAI & Agentic AI Developer | Building AI Agents, Local LLM Applications, RAG Systems & Workflow Automation</h3>

<p align="center">
  <a href="https://linkedin.com/in/avaneeshjoshi18"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:avaneeshjoshi18@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://avaneeshportfolio.netlify.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=netlify&logoColor=white"/></a>
  <a href="https://github.com/Avaneesh635"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>

---

##  About Me

AI/ML Engineer who has independently shipped 10+ production-grade AI systems, from a self-healing agentic RAG system to an offline desktop AI assistant. Active open-source contributor with 7 merged pull requests to a LangGraph-based Playwright self-healing engine — including three maintainer-rated "Core Feature" implementations.

Interested in: Generative AI Engineering · Applied AI · Agentic AI · RAG Systems · AI Automation · Forward Deployed Engineering

 Fresher | Open to Full-Time Opportunities | Open to Relocation

---

##  Open Source Contributions

### E2E-Self-Heal — LangGraph/Playwright Self-Healing Engine

> 7 merged pull requests into a public production codebase, progressing from test coverage to core-feature architecture — promoted from Contributor to Collaborator by the maintainer.

- Built a deterministic **MatchScorer** (Python) for network-mock replay using weighted similarity scoring across URL, headers, query params, and body, with tie-breaking logic for reproducibility
- Built a persistent **SnapshotStore** (Pydantic schemas, structlog logging, custom exception hierarchy) for Shadow Runtime state — rated **"Core Feature"** by the maintainer
- Built the **Playwright Mock Injector** for the Shadow Testing system, handling sync/async Playwright runtimes via route interception — also rated **"Core Feature"**
- Wired end-to-end **Shadow Runtime replay orchestration** (`run_shadow()`), launching headless Chromium and connecting Playwright via a remote-debugging websocket — called a critical feature by the maintainer
- Added a **shadow-verify node** gating patches through deterministic offline replay before live test runs, wired into the core self-healing LangGraph workflow — rated **"Core Feature"**
- Replaced a regex-based JSX diff parser with a **tree-sitter AST parser**, with graceful fallback, to make selector-diff analysis robust against complex nested JSX
- Added **70+ pytest unit tests** across CLI, selector verification, and sandboxed runner modules, including a cross-platform Windows symlink fix

**Repo:** [Lee-Dongwook/E2E-Self-Heal](https://github.com/Lee-Dongwook/E2E-Self-Heal)

---

##  Featured Projects

###  DocOps Agent — Self-Healing RAG System

> *Built a self-healing agentic RAG system that automatically detects and corrects its own failed answers instead of returning them silently, as measured by an automatic-retry loop triggered whenever an answer fails a faithfulness/relevance check, by architecting a LangGraph state machine wrapping a pgvector retrieval pipeline with a Redis semantic cache.*

- Designed a LangGraph agent (retrieve → reason → verify) with a self-healing loop that automatically retries with an altered retrieval strategy when an answer fails evaluation, instead of returning it unflagged
- Built a Redis semantic caching layer in front of a pgvector HNSW retrieval pipeline to cut repeat-query latency and eliminate redundant LLM spend
- Reduced ungrounded responses via a Ragas-style faithfulness and relevance evaluator, with prompt-injection guardrails gating every answer before it reaches the user

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=for-the-badge)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Repo:** [Avaneesh635/DocOps-Agent](https://github.com/Avaneesh635/DocOps-Agent)

---

###  AI Business Operations Copilot

> *Consolidated 5+ business functions into a single zero-intervention pipeline, as measured by elimination of separate tools for lead intelligence, support triage, and meeting intelligence, by architecting a unified AI platform using n8n Switch nodes with LLM-structured outputs feeding live Google Sheets dashboards.*

- Reduced manual reporting time by ~70%, as measured by time-to-dashboard dropping from 2+ hours to under 5 minutes, by automating lead scoring, sentiment classification, and priority detection end-to-end
- Processed 100+ requests per workflow run with zero manual intervention, as measured by end-to-end automation rate, by designing a fully orchestrated pipeline with no human touchpoints

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge)
![Groq](https://img.shields.io/badge/Groq_LLM-00C853?style=for-the-badge)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-FF6B6B?style=for-the-badge)
![Workflow Automation](https://img.shields.io/badge/Workflow_Automation-2196F3?style=for-the-badge)

---

###  Luna — AI-Powered Personal Desktop Assistant

> *Delivered a privacy-first desktop assistant running entirely offline, as measured by zero external API calls across chat, memory, and automation features, by architecting an Electron + React app powered by a local Ollama LLM daemon with a secure ContextBridge IPC layer.*

- Enabled safe hands-off OS automation, as measured by every system-level action (email drafting, file organizing, batch renaming, app launching) requiring explicit click-to-grant consent, by building sandboxed automation modules gated behind consent security modals
- Built a self-updating personal memory layer, as measured by automatic extraction of user preferences and facts during natural conversation, by implementing agentic memory extraction with a searchable, editable local memory dashboard

**Tech Stack**

![Electron](https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge)
![Web Audio API](https://img.shields.io/badge/Web_Audio_API-FF6B6B?style=for-the-badge)

---

###  Redis-Lite — Asynchronous Concurrent Key-Value Store

> *Delivered a high-performance, asynchronous in-memory key-value store, as measured by successful command execution (GET, SET, DEL, EXISTS, PING) and seamless compatibility with the official redis-cli tool, by architecting a multi-threaded TCP server in Rust powered by the Tokio runtime.*

- Eliminated lock contention under heavy concurrent read/write traffic, as measured by independent lock acquisition across partitions, by implementing a database sharding engine splitting data store state across 16 memory shards protected by separate RwLocks
- Prevented thread starvation and request blocking during active key eviction, as measured by zero-overhead key cleanups, by designing a background TTL garbage collection worker that utilizes non-blocking try_write locks to prune expired keys

**Tech Stack**

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Tokio](https://img.shields.io/badge/Tokio-E06F3F?style=for-the-badge)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![RESP Protocol](https://img.shields.io/badge/RESP_Protocol-FF6B6B?style=for-the-badge)
![Multi Threading](https://img.shields.io/badge/Multi_Threading-2196F3?style=for-the-badge)

---

##  Tech Stack

### Languages
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### AI & Automation
![Generative AI](https://img.shields.io/badge/Generative_AI-412991?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Groq](https://img.shields.io/badge/Groq_LLM-00C853?style=for-the-badge)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-000000?style=for-the-badge)
![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=for-the-badge)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-FF6B6B?style=for-the-badge)
![Agentic AI](https://img.shields.io/badge/Agentic_AI-FF6B6B?style=for-the-badge)
![Ragas](https://img.shields.io/badge/Ragas_Evaluation-00C853?style=for-the-badge)
![LLM Guardrails](https://img.shields.io/badge/LLM_Guardrails-C0392B?style=for-the-badge)
![MediaPipe](https://img.shields.io/badge/MediaPipe-00C853?style=for-the-badge)
![REST APIs](https://img.shields.io/badge/REST_APIs-FF6B6B?style=for-the-badge)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B6B?style=for-the-badge)
![Gmail API](https://img.shields.io/badge/Gmail_API-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)

### ML & Computer Vision
![Scikit Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-00C853?style=for-the-badge)
![Sentence Transformers](https://img.shields.io/badge/Sentence_Transformers-FF6B6B?style=for-the-badge)

### Frameworks & Tools
![Tokio](https://img.shields.io/badge/Tokio-E06F3F?style=for-the-badge)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions_CI/CD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

### Databases
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=for-the-badge)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)

---

##  Certifications
-  Google Cloud Certified Professional Machine Learning Engineer
-  AWS Cloud Practitioner Certified
-  Oracle Agentic AI Certified

---

##  Connect With Me
 LinkedIn: https://linkedin.com/in/avaneeshjoshi18  
 Email: avaneeshjoshi18@gmail.com  
 GitHub: https://github.com/Avaneesh635  
 Portfolio: https://avaneeshportfolio.netlify.app
