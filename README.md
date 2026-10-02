# gienini2

**AI systems builder** · **AI Security & offensive security (in training)** · Law enforcement professional · Ex-PLC programmer (Omron, international deployments)

> Built 18+ production AI systems independently in 6 months — FinTech, GovTech, industrial RAG, local AI infrastructure, and RPA automation. Now specializing in **AI Security / LLM red teaming** and **ethical hacking**.

---

## What I build

I come from industrial automation (PLC programming, international deployments in Pakistan, Madrid, Barcelona) and 18 years in law enforcement. Since late 2025 I've been applying that systems-thinking mindset to AI — building real, deployed tools that solve real operational problems — and I'm now moving into **offensive security**, where my AI background and systems experience meet.

No tutorials. No toy projects. Everything here runs in production or was built for a specific operational need.

---

## Projects

### 🛡️ Security / Offensive

| Project | What it does | Status |
|---------|-------------|--------|
| `METATRON` | AI-powered pentesting assistant (CLI). Automates the engagement cycle: **recon → vulnerability-pattern recognition → advisory attack-tree**. A local LLM writes the report while the code owns the ground truth (version-filtered `searchsploit` cross-referencing) with anti-hallucination guardrails. Validated against ~200 vulnerable lab machines | In development |

**Focus:** AI Security / LLM red teaming (OWASP Top 10 for LLM) · web & network pentesting
**Learning path:** eJPT → PNPT → OSCP
**Stack:** Kali Linux · `nmap` / `rustscan` · Metasploit · `searchsploit` · web exploitation (SQLi/LFI/upload) · privilege escalation · Docker labs

---

### ⚡ FinTech / Trading Systems

| Repo | What it does | Status |
|------|-------------|--------|
| [`tingbot_binance`](https://github.com/gienini2/tingbot_binance) | Algorithmic trading bot on Binance (BTCUSDC, M1). 6-module pipeline: signal detector → thermometer → weather model → decision engine → watchdog → capital manager. 24/7 autonomous operation with Telegram alerts | Production |
| `tickbot` | Tick-level signal processor and order manager | Production |
| `trading-agent-v1` | First-generation trading agent with real-time chart generation and automated signal visualization | Production |

**Stack:** Python · Binance API · systemd · Hetzner VPS · Telegram Bot API

---

### 🏛️ GovTech / LegalTech

> Built for real public-administration operations. Source and data are **private** (sensitive operational systems) — happy to walk through the architecture in an interview.

| Project | What it does | Status |
|---------|-------------|--------|
| `bitacola` | Operations-management platform for a municipal police force. Self-hosted (Debian · Nginx · PM2 · SSL · private mesh VPN) | Production · Private |
| `sherlock` | AI document-generation engine — the officer dictates and an LLM produces legally-formatted official reports in real time (FastAPI) | Production · Private |
| `penal` | Legal-code lookup and behavioural pattern analysis using embeddings + cosine similarity | Production · Private |
| `central-partes` | Unified command panel: photo ingestion, AI cataloging, auto-formatting to the official report standard | Production · Private |
| `iactes` | Digital creation and management of municipal infringement records, with integrated reference management | Production · Private |
| `photo-evidence-manager` | Desktop app that cross-references field photos with case CSVs; automatic file indexing (Watchdog) | Production · Private |
| `legacy-migration` | Migration of a legacy Access/VBA municipal management system (~40 tables) to Python + SQLite | Legacy / Migration · Private |
| [`OPOS`](https://github.com/gienini2/OPOS) | Daily scraper of **public** municipal notice boards (*taulell d'edictes*) — automated detection of civil-service exam announcements with instant alerts | Production |
| `firmadoc-monitor` | Playwright automation of a municipal BPM platform: daily monitoring of records, Excel extraction, Telegram alerts | Development · Private |

**Stack:** Python · Node.js · FastAPI · Express.js · SQLite · docxtemplater · python-docx · Playwright · Tkinter · Watchdog · Anthropic API · Nginx · PM2 · Telegram Bot API

---

### 🏗️ Engineering / RAG

| Repo | What it does | Status |
|------|-------------|--------|
| `bafatec-rag` | Production RAG system over ~5,000 industrial engineering project files — vector search, receipt OCR/cataloging, and automated technical report generation | Production |
| `whatsapp-to-project` | Processes exported WhatsApp conversations (audio + text) to auto-extract and structure the data for a full electrical-engineering project. Whisper STT + domain-specific LLM extraction pipeline. Validated with local Llama and Nvidia API | Local / demo available |

**Stack:** Python · Embeddings · Vector DB · OCR · Whisper/STT · Anthropic API · Document generation

---

### 🧠 Local AI Infrastructure

| Repo | What it does | Status |
|------|-------------|--------|
| `jarvis-cognitive` | Local cognitive assistant on Ollama (Llama 3.2 / Qwen 2.5). On-premise, zero data egress. GPU node available (RTX-class) for scaling | Active |

**Stack:** Ollama · Llama 3.2 · Qwen 2.5 · Python · Linux Debian · Local-first architecture

---

### 🏃 Health / Quantified Self

| Repo | What it does | Status |
|------|-------------|--------|
| [`Alpha50-core`](https://github.com/gienini2/Alpha50-core) | Personal fitness and weight tracking agent — MVP complete, on standby | Standby |

---

## Infrastructure & Cloud

Self-hosted production infrastructure (Linux Debian · Nginx · systemd · PM2 · SSL · private mesh VPN) plus a GPU inference node (RTX-class) for local LLMs.

**Cloud platforms:** AWS (EC2 · 24/7 trading bots) · Google Cloud · Hetzner VPS

---

## Technical profile

```
LLM Integration        ████████████  Production (Anthropic API, Ollama)
RAG / Vector Search    ████████████  Production (5,000+ file corpus)
Agent Orchestration    ██████████░░  Multi-agent systems
Web Automation / RPA   ████████████  Playwright, Watchdog, scraping, BPM
Server Deployment      ████████████  AWS · Google Cloud · Hetzner · self-hosted Debian
API Development        ████████████  FastAPI, Express.js, REST, webhooks
Document Generation    ██████████░░  Word/docxtemplater, AI-personalized records
Audio / STT Pipeline   ████████░░░░  Whisper, conversation parsing, data extraction
Trading Systems        ████████░░░░  Binance API, 6-module signal pipeline
Local LLM / GPU        ████████░░░░  Ollama, RTX-class node (expanding)
AI Security / LLM RT   ████░░░░░░░░  Learning (OWASP Top 10 for LLM, prompt injection)
Offensive Security     ███░░░░░░░░░  Learning (eJPT → PNPT → OSCP · ~200 labs)
Industrial Automation  ████████████  PLC Omron (Ladder), SCADA, Syswin
Database Design        ████████████  SQLite, relational design (40+ table systems)
```

**Languages:** Python · Node.js · JavaScript · SQL · VBA/Access · Visual Basic · Ladder (PLC Omron)
**Security:** pentesting (web & network) · nmap/rustscan · Metasploit · searchsploit · privesc · LLM security
**Cloud:** AWS (EC2) · Google Cloud · Hetzner VPS · private mesh VPN
**Infrastructure:** Linux Debian · Nginx · systemd · cron · SSH · PM2 · Docker
**AI/ML:** Anthropic API · Nvidia API · OpenAI API · Ollama · Whisper · Prompt engineering · RAG · Agents

---

## Background

- 🚓 **Active law enforcement officer** — Policia Local, Catalonia (18 years, including team lead)
- 🏭 **Former PLC programmer** — Omron automation, international deployments (Pakistan, Madrid, Barcelona)
- 📐 **Physics degree (UNED)** — strong mathematical and analytical foundation
- 🥋 **1st Dan black belt, Taekwondo**
- 🌍 **Languages:** Catalan (C1 certified) · Spanish (native) · English (technical/intermediate)

---

## What I'm looking for

Roles where domain expertise meets AI engineering and security:

- **AI Security Engineer / LLM red teaming** — securing and testing AI systems
- **Penetration Tester** (junior) — offensive security, ethical hacking
- **AI Engineer** — building and deploying LLM-based systems
- **Automation / RPA Engineer** — intelligent process automation
- **GovTech / LegalTech** — AI for public administration or legal workflows

Open to remote. Based in Catalonia, Spain.

📫 Reach me via GitHub or LinkedIn.
