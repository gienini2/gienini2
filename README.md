# gienini2

**AI systems builder** · Law enforcement professional · Ex-PLC programmer (Omron, international deployments)

> Built 15+ production AI systems independently in 6 months — FinTech, GovTech, industrial RAG, local AI infrastructure, and RPA automation.

---

## What I build

I come from industrial automation (PLC programming, international deployments in Pakistan, Madrid, Barcelona) and 18 years in law enforcement. Since November 2025 I've been applying that systems-thinking mindset to AI — building real, deployed tools that solve real operational problems.

No tutorials. No toy projects. Everything here runs in production or was built for a specific operational need.

---

## Projects

### ⚡ FinTech / Trading Systems

| Repo | What it does | Status |
|------|-------------|--------|
| [`tingbot_binance`](https://github.com/gienini2/tingbot_binance) | Algorithmic trading bot on Binance (BTCUSDC, M1). 6-module pipeline: signal detector → thermometer → weather model → decision engine → watchdog → capital manager. 24/7 autonomous operation with Telegram alerts | Production |
| `tickbot` | Tick-level signal processor and order manager | Production |
| `trading-agent-v1` | First-generation trading agent with real-time chart generation and automated signal visualization | Production |

**Stack:** Python · Binance API · systemd · Hetzner VPS · Telegram Bot API

---

### 🏛️ GovTech / LegalTech

| Repo | What it does | Status |
|------|-------------|--------|
| [`bitacola-backend`](https://github.com/gienini2/bitacola-backend) | Core of Bitácola — full police operations management system. Self-hosted on Debian with Nginx, PM2, SSL, 6-node Tailscale mesh network | Production |
| [`sherlock-backend`](https://github.com/gienini2/sherlock-backend) | AI document generation engine — officer speaks, LLM generates legally-formatted official Catalan police reports in real time. FastAPI backend over 1,200+ person/vehicle records | Production |
| [`penal_backend`](https://github.com/gienini2/penal_backend) | Criminal code lookup and behavioural pattern analysis using cosine similarity and behaviour vectors | Production |
| `central-partes` | Unified command panel: photo ingestion, AI cataloging, auto-DRAG formatting (official Catalan police report standard), aggregates reports across municipalities | Production |
| [`iactes-arboreo`](https://github.com/gienini2/iactes-arboreo) | Digital creation and management of infringement records (I-actes) for Ajuntament de l'Arboç, with integrated NPN management | Production |
| `photo-evidence-manager` | Windows desktop app: cross-references expedition photos with fine/complaint CSVs. Automatic file indexing with Watchdog | Production |
| `figaro-guard-system` | Legacy police management system for Figaró-Montmany municipal police. Built in Access/VBA: 42 tables, ~800 citizens, ~400 vehicles, ~20 officers. Currently in migration to Python + SQLite | Legacy / Migration |
| [`OPOS`](https://github.com/gienini2/OPOS) | Daily scraper monitoring official municipal notice boards (*taulell d'edictes*) across multiple Catalan municipalities — automated detection of civil service exam announcements with instant alerts | Production |
| `firmadoc-monitor` | Playwright-based automation of a municipal BPM platform (Berger Levraut). Daily monitoring of administrative entry records, Excel extraction, and Telegram alerts | Development |

**Stack:** Python · Node.js · FastAPI · Express.js · SQLite · Access/VBA · docxtemplater · python-docx · Playwright · Tkinter · Watchdog · Anthropic API · Nginx · PM2 · Tailscale · Telegram Bot API

---

### 🏗️ Engineering / RAG

| Repo | What it does | Status |
|------|-------------|--------|
| `bafatec-rag` | Production RAG system over ~5,000 industrial engineering project files — vector search, receipt OCR/cataloging, and automated technical report generation for BAFATEC Industrial SL | Production |
| `whatsapp-to-project` | Processes exported WhatsApp conversation ZIP files (audio + text) to automatically extract and structure all the data required to populate a full electrical engineering project — client requirements, site conditions, materials, regulatory details. Whisper STT + domain-specific LLM extraction pipeline. Validated with local Llama and Nvidia API | Local / demo available |

**Stack:** Python · Embeddings · Vector DB · OCR · Whisper/STT · Anthropic API · Document generation

---

### 🧠 Local AI Infrastructure

| Repo | What it does | Status |
|------|-------------|--------|
| `jarvis-cognitive` | Local cognitive assistant on Ollama (Llama 3.2 / Qwen 2.5). On-premise, zero data egress. Tested with local Llama inference and Nvidia API. GPU node available (RTX 5050) for scaling | Active |

**Stack:** Ollama · Llama 3.2 · Qwen 2.5 · Python · Linux Debian · Local-first architecture

---

### 🏃 Health / Quantified Self

| Repo | What it does | Status |
|------|-------------|--------|
| [`Alpha50-core`](https://github.com/gienini2/Alpha50-core) | Personal fitness and weight tracking agent — MVP complete, on standby | Standby |

---

## Infrastructure

**Bitácola private mesh** (Tailscale + Nginx + SSL — Figaró deployment):

```
figaro-server    · Linux Debian · Primary server · Nginx · PM2 · production
workstation-gpu  · HP Victus · RTX 5050 · GPU inference node
workstation-dev  · Secondary development workstation
mobile-node-1    · iPhone 13
mobile-node-2    · Android (Motorola G85)
```

**Cloud platforms used:**

```
AWS              · EC2 · First trading bots (24/7 production)
Google Cloud     · Various services
Hetzner VPS      · TingBot · current trading production · beta services
```

---

## Technical profile

```
LLM Integration        ████████████  Production (Anthropic API, Ollama)
RAG / Vector Search    ████████████  Production (5,000+ file corpus)
Agent Orchestration    ██████████░░  Multi-agent systems (Bitácola ecosystem)
Web Automation / RPA   ████████████  Playwright, Watchdog, scraping, BPM
Server Deployment      ████████████  AWS · Google Cloud · Hetzner · self-hosted Debian
API Development        ████████████  FastAPI, Express.js, REST, webhooks
Document Generation    ██████████░░  Word/docxtemplater, AI-personalized records
Audio / STT Pipeline   ████████░░░░  Whisper, WhatsApp ZIP parsing, data extraction
Trading Systems        ████████░░░░  Binance API, 6-module signal pipeline
Local LLM / GPU        ████████░░░░  Ollama, RTX 5050 (expanding)
Industrial Automation  ████████████  PLC Omron (Ladder), SCADA, Syswin
Database Design        ████████████  SQLite, Access/VBA (42-table production system)
```

**Languages:** Python · Node.js · JavaScript · SQL · VBA/Access · Visual Basic · Ladder (PLC Omron)
**Databases:** SQLite · Access · MySQL
**Cloud:** AWS (EC2, 24/7 trading bots) · Google Cloud · Hetzner VPS · Tailscale (private mesh, Bitácola deployment)
**Infrastructure:** Linux Debian · Nginx · systemd · cron · SSH · PM2 · Docker (basic)
**AI/ML:** Anthropic API · Nvidia API · OpenAI API · Ollama · Whisper · Prompt engineering · RAG · Agents

---

## Background

- 🚓 **Active law enforcement officer** — Policia Local, Catalonia (18 years, including team lead)
- 🏭 **Former PLC programmer** — Omron automation, international deployments (Pakistan, Madrid, Barcelona)
- 📐 **Physics degree (UNED)** — strong mathematical and analytical foundation
- 🥋 **1st Dan black belt, Taekwondo**
- 🌍 **Languages:** Catalan (C1 certified) · Spanish (native) · English (technical/intermediate)

*Extended development period Feb–Oct 2025, then continued from November 2025 — this repository is what came out of it.*

---

## What I'm looking for

Roles where domain expertise meets AI engineering:

- **AI Engineer** — building and deploying LLM-based systems
- **Automation / RPA Engineer** — intelligent process automation
- **GovTech / LegalTech** — AI for public administration or legal workflows
- **FinTech** — trading systems, financial data pipelines

Open to remote. Based in Catalonia, Spain.

📫 Reach me via GitHub or LinkedIn.
