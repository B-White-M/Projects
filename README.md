# Byron White — Data & AI Engineering

> Production AI agents built on real data infrastructure — ETL, RAG, and vector search, not chatbot wrappers.

I design and ship AI systems that execute real business actions: conversational commerce agents, retrieval-augmented inventory search, and the data pipelines that make them reliable. My approach is data-first — the intelligence layer is only as good as the structured data underneath it.

This repository indexes selected work across applied AI, data engineering, security architecture, and business intelligence.

**Focus areas:** Agentic AI · RAG & vector search · Workflow orchestration · Data modeling · Multi-tenant security · BI & automation

---

## Featured — Applied AI

### AI Conversational Commerce Orchestrator · 2025–2026

**Repo:** [mom-ia-PUBLIC](https://github.com/B-White-M/mom-ia-PUBLIC)

An end-to-end AI agent that automates WhatsApp sales operations — answering product questions in natural language, building carts, generating quotes, and escalating to a human when needed.

**Stack**

- **n8n** (self-hosted) for event-driven workflow orchestration
- **Claude API** for reasoning — Haiku for intent classification, Sonnet for response generation — using tool calling (function calling with JSON schemas) so the model returns structured actions, not free text
- **Supabase (PostgreSQL + pgvector)** for structured storage and semantic vector search
- **OpenAI** for multimodal input — Whisper (audio), Vision (images), and embeddings (`text-embedding-3-small`)
- **Meta Cloud API (WhatsApp Business API)** as the messaging channel

**Key capabilities**

- Natural-language inventory search via RAG (semantic, not keyword matching)
- Intent detection and tool-based routing
- Multimodal understanding — text, voice notes, and images
- Cart handling and structured quote generation
- Deterministic business logic — inventory and state changes handled outside the LLM layer
- Human escalation with conversation summarization
- Multi-tenant isolation via Row-Level Security (RLS)

Demonstrates applied AI, event-driven architecture, and production-ready data modeling.

---

## Data Engineering & Security

### Row-Level Security (RLS) Architecture for Tabular Models · 2025

**Repo:** [tabular-rls-multi-level-security](https://github.com/B-White-M/tabular-rls-multi-level-security)

Design and implementation of a scalable, multi-level security architecture for enterprise tabular models, built on dimensional hierarchies and filter propagation.

Covers hierarchical security design, security tables, superuser access patterns, filter propagation, and impersonation testing.

---

## Business Intelligence & Analytics

### Global Assets Dashboard — Power BI · 2023–2024

**Repo:** [Global_Assets_Dashboard](https://github.com/B-White-M/Global_Assets_Dashboard)

Power BI solution that analyzes and visualizes asset-management data, surfaces recurring errors and financial risk, and includes a real-time location map connected to a SQL backend to support decision-making.

---

## Foundations — Data & Automation

### Python — Web Scraping & Market Analysis · 2023–2024

**Repo:** [Python / Jupyter](https://github.com/B-White-M/Pyton-Jupyter-)

Web scraping across multiple sources to gather market-trend data, then analyzing supply-and-demand drivers over time.

### VBA — Excel Automation · 2022–2023

**Repo:** [VBA-Excel-Macros](https://github.com/B-White-M/VBA-Excel-Macros)

Form-driven data capture into structured spreadsheets, plus automated personalized email dispatch from Excel via VBA.

---

## Tech Stack

- **AI / LLM:** Claude API (tool use, RAG), OpenAI (Whisper, Vision, embeddings)
- **Data:** PostgreSQL, Supabase, pgvector, SQL, ETL
- **Orchestration:** n8n
- **BI & Analytics:** Power BI, DAX, Python (Pandas)
- **Channels & APIs:** Meta Cloud API (WhatsApp Business), REST API integration

---

## Contact

- **Email:** byron.w.montero@gmail.com
- **LinkedIn:** [byron-white-montero](https://www.linkedin.com/in/byron-white-montero-069422123)
