<h1 align="center">Hi 👋, I'm Avaneesh Joshi</h1>
<h3 align="center">AI/ML Engineer | GenAI & Agentic AI Developer | Building AI Agents, Local LLM Applications, RAG Systems & Workflow Automation</h3>

<p align="center">
  <a href="https://linkedin.com/in/avaneeshjoshi18"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:avaneeshjoshi18@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://avaneeshportfolio.netlify.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=netlify&logoColor=white"/></a>
  <a href="https://github.com/Avaneesh635"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>

---

## 🚀 About Me

I'm a self-taught AI/ML Engineer who has independently shipped 10+ production-grade AI systems, from a hardened Generative AI RAG API to an offline desktop AI assistant. I'm also an active open-source contributor, with 5 merged pull requests to a LangGraph-based Playwright self-healing engine — including two maintainer-rated "Core Feature" implementations.

I enjoy designing production-ready AI applications that combine modern LLMs with automation platforms, APIs, vector databases, desktop applications, and cloud services — turning them into systems that solve real-world problems, from autonomous business workflows to local-first AI assistants.

🎯 Interested in:
- Generative AI Engineering
- Applied AI
- Agentic AI
- RAG Systems
- AI Automation
- AI Platform Engineering
- Forward Deployed Engineering

📍 Fresher | Open to Full-Time Opportunities | Open to Relocation

---

## 🌱 Open Source Contributions

### E2E-Self-Heal — LangGraph/Playwright Self-Healing Engine

> 5 merged pull requests into a public production codebase, progressing from test coverage to core-feature architecture — promoted from Contributor to Collaborator by the maintainer.

- Built a deterministic **MatchScorer** (Python) for network-mock replay using weighted similarity scoring across URL, headers, query params, and body, with tie-breaking logic for reproducibility
- Built a persistent **SnapshotStore** (Pydantic schemas, structlog logging, custom exception hierarchy) for Shadow Runtime state — rated **"Core Feature"** by the maintainer
- Built the **Playwright Mock Injector** for the Shadow Testing system, handling sync/async Playwright runtimes via route interception — also rated **"Core Feature"**
- Replaced a regex-based JSX diff parser with a **tree-sitter AST parser**, with graceful fallback, to make selector-diff analysis robust against complex nested JSX
- Added **70+ pytest unit tests** across CLI, selector verification, and sandboxed runner modules, including a cross-platform Windows symlink fix

**Repo:** [Lee-Dongwook/E2E-Self-Heal](https://github.com/Lee-Dongwook/E2E-Self-Heal)

---

## 🏆 Featured Projects

### 🛡️ Production RAG API — Hardened Retrieval System

> *Reduced repeat-query latency from ~150ms to ~1ms and eliminated redundant LLM spend, as measured by semantic cache hit rate, by building an embedding-similarity cache layer in front of a hardened, production-grade Generative AI Retrieval-Augmented Generation API.*

- Enabled zero-code-change deployment across dev and production, as measured by identical test suites passing in both environments, by architecting a dual-mode vector store interface that swaps an in-memory NumPy backend for a pgvector/PostgreSQL HNSW index
- Reduced ungrounded and unsafe responses, as measured by automated faithfulness and grounding scores from a custom Ragas-style evaluation suite, by layering prompt-injection detection, document-poisoning checks, and hallucination guardrails around every generated answer
- Cut manual eval effort to near-zero, as measured by automated scoring on every pipeline change, by building a repeatable `run_evals.py` harness reporting faithfulness, grounding, and routing accuracy

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=for-the-badge)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Ragas](https://img.shields.io/badge/Ragas_Evaluation-00C853?style=for-the-badge)

---

### 🌙 Luna — AI-Powered Personal Desktop Assistant

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

### 🤖 AI Business Operations Copilot

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

### ⚡ Redis-Lite — Asynchronous Concurrent Key-Value Store

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

### 🧠 AI Meeting Intelligence Assistant

> *Eliminated manual note-taking and follow-up tracking entirely, as measured by automated extraction of action items, risks, and recommendations from raw meeting transcripts, by building an AI pipeline using Gemini AI with structured prompt engineering to parse and surface insights in seconds.*

- Reduced post-meeting processing time from hours to under a minute, as measured by time from transcript input to structured output, by chaining summarization, action detection, and risk identification into a single Streamlit workflow
- Improved follow-up reliability, as measured by zero missed action items across tested meetings, by using LLM-based detection rather than manual review

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![APIs](https://img.shields.io/badge/APIs-FF6B6B?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-00C853?style=for-the-badge)

---

### 🎯 AI Lead Research Agent

> *Reduced lead qualification time by ~65%, as measured by time per qualified lead vs. manual research, by automating the full sales intelligence cycle — company enrichment, opportunity discovery, lead scoring, and personalized outreach — via n8n and Groq LLM.*

- Eliminated manual research steps entirely, as measured by zero human intervention per lead, by chaining REST API calls with LLM reasoning to produce structured lead profiles and ready-to-send outreach automatically
- Delivered structured lead reports to Google Sheets in real time, as measured by instant dashboard updates per workflow run, by routing LLM-generated outputs directly into live spreadsheets via API

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge)
![Groq](https://img.shields.io/badge/Groq_LLM-00C853?style=for-the-badge)
![REST APIs](https://img.shields.io/badge/REST_APIs-FF6B6B?style=for-the-badge)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)

---

### 🎫 AI Support Ticket Classifier

> *Automated support triage end-to-end, as measured by tickets being classified, prioritized, and responded to without human intervention, by building an n8n workflow with Gemini AI handling classification, priority detection, response generation, and escalation routing.*

- Cut first-response time to near-zero, as measured by auto-generated responses triggered immediately on ticket receipt via webhook, by connecting intake webhooks directly to LLM inference and Google Sheets logging
- Improved routing accuracy, as measured by consistent priority and escalation labels across ticket types, by engineering structured prompts that output machine-readable classification fields

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B6B?style=for-the-badge)

---

### 📧 AI Email Automation Agent

> *Automated the full email management cycle, as measured by classification, summarization, action extraction, and draft generation happening without manual reading, by building a Streamlit + Gemini AI pipeline connected to Gmail API with webhook-triggered processing.*

- Reduced email triage time to near-zero, as measured by instant classification and priority detection on inbox events, by triggering LLM inference automatically on new message webhooks
- Generated ready-to-send response drafts, as measured by structured output per email thread, by prompting Gemini AI with full thread context and extracting action items and follow-up recommendations in a single pass

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Gmail API](https://img.shields.io/badge/Gmail_API-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B6B?style=for-the-badge)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-00C853?style=for-the-badge)

---

### 📄 AI Resume Analyzer & Optimizer

> *Delivered ATS score, skill gap analysis, and optimization recommendations in seconds, as measured by structured report generation from a raw resume + job description pair, by building a Gemini AI pipeline with NLP-based parsing and PDF processing.*

- Enabled job-specific resume targeting, as measured by per-JD match scoring and tailored suggestions, by prompting the LLM with both resume content and job description simultaneously for comparative analysis
- Reduced manual resume review effort to zero, as measured by instant ATS scoring without human evaluation, by automating the full parsing-to-recommendation pipeline in a single Streamlit interface

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-00C853?style=for-the-badge)
![PDF Processing](https://img.shields.io/badge/PDF_Processing-FF6B6B?style=for-the-badge)

---

### 🎭 Emotion Lens — Real-Time Facial Emotion Recognition

> *Delivered real-time emotion detection (Happy, Sad, Surprised) with live confidence scores in the browser, as measured by end-to-end WebSocket latency from webcam frame to predicted result, by streaming base64 frames from the browser to a Flask-SocketIO server running in-memory MediaPipe inference.*

- Achieved robust landmark-based classification using 1,434 normalised facial coordinates per frame, as measured by per-class precision and recall on a held-out 20% test set, by training a 200-tree Random Forest on 478-point MediaPipe face landmarks with stratified splitting
- Built a zero-data-retention pipeline deployable on any local network device, as measured by full inference running at http://\<ip\>:5000 with no files written to disk, by processing and discarding every frame entirely in memory

**Tech Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-00C853?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![SocketIO](https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

---

## 💻 Tech Stack

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

## 📜 Certifications
- 🏆 Google Cloud Certified Professional Machine Learning Engineer
- ☁️ AWS Cloud Practitioner Certified
- 🤖 Oracle Agentic AI Certified

---

## 🌍 Connect With Me
💼 LinkedIn: https://linkedin.com/in/avaneeshjoshi18  
📧 Email: avaneeshjoshi18@gmail.com  
🐙 GitHub: https://github.com/Avaneesh635  
🌐 Portfolio: https://avaneeshportfolio.netlify.app
