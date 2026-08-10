# Kiarash Adl | AI-Native Software Architect

**Building safe infrastructure for the agentic era.**

I design and ship privacy-first, agent-ready systems — from on-device iOS applications to remote Model Context Protocol (MCP) servers. My work sits at the intersection of zero-knowledge encryption, immutable audit trails, and developer-facing AI tooling.

📍 Nassau Bay, Texas &nbsp;·&nbsp; 🌐 [25x.codes](https://25x.codes) &nbsp;·&nbsp; 🔧 [mcp.undisk.app](https://mcp.undisk.app)

---

## Core Philosophy

- **Spec-Driven Development (SDD)** — Every feature begins as a machine-readable spec before a single line of code is written. Specifications are the source of truth; code is a derived artifact.
- **Privacy-First Architecture** — Data stays on-device or under user control. Zero-knowledge encryption and scoped access are defaults, not afterthoughts.
- **Undo-First Infrastructure** — AI agents need the power to act and the safety net to reverse. Every mutation is versioned, auditable, and reversible in under 50 ms.

---

## Experience

### Engineer · STLabs

Built MCP for [stlabs.com](https://stlabs.com), bringing STLabs service-management workflows into the AI assistants where investigations begin. Agents authenticate through the user's STLabs account, inherit existing permissions and visibility rules, and leave actions in the same audit trail as all other work.

→ [**Bring Your Own Agent: Introducing mcp.stlabs.com**](https://stlabs.com/engineering/bring-your-own-agent)

---

## Flagship Projects

### 🔐 [Undisk MCP](https://mcp.undisk.app) — The Undo-First File Workspace for AI Agents

The safest way to let AI agents work with files. Undisk MCP is a remote MCP server that gives Claude, Cursor, Copilot, and any MCP-compatible agent scoped, reversible access to a versioned file workspace — so they can read, write, and search without ever becoming a dangerous "delete everything" bot.

| Capability | Detail |
|---|---|
| **20+ MCP tools** | File CRUD, versioning, undo, diff, search, policy engine, secret vault, tamper-evident audit trail, E2B compute sandbox |
| **Per-file undo** | Restore any file to any prior version without rolling back the entire workspace |
| **WebSocket transport** | 4 ms reads, 19 ms writes — persistent connection with zero idle billing via Cloudflare Durable Objects + Hibernation API |
| **Zero-knowledge secret vault** | Encrypted at rest, agent-scoped, never in file listings or search results |
| **Policy engine** | Path-based ACLs, file-size limits, rate caps, anomaly alerts — configurable per workspace |
| **Secret detection** | 20+ patterns (AWS keys, GitHub PATs, private keys) scanned and blocked on every write |
| **Tamper-evident audit trail** | Every operation logged with agent identity, content hash, and hash-chain integrity verification |
| **EU AI Act readiness** | Immutable versioning + audit trail enables deployer compliance with Articles 12, 14, and 26 |

**Architecture:** Cloudflare Workers (Smart Placement) → Durable Objects (one per workspace, SQLite + R2) → content-addressable storage with SHA-256 deduplication. Dual-provider with Fastly edge compute for read-heavy workloads.

**Integrations:** Claude Desktop · Cursor · VS Code · GitHub Copilot · Google ADK · LlamaIndex · LangChain · Docker MCP Hub

→ [**mcp.undisk.app**](https://mcp.undisk.app) &nbsp;|&nbsp; [Get started](https://mcp.undisk.app/signup) &nbsp;|&nbsp; [Live demo](https://mcp.undisk.app/e2b)

---

### 📖 [Bayan](https://trybayan.com) — Bilingual Persian Poetry Analysis (iOS)

The only app providing bilingual Farsi-English literary analysis of classical Persian poetry. Bayan decodes Sufi symbolism, historical allusions, and archaic vocabulary — fully offline with verse text sourced from a verified canonical corpus, not AI-generated.

| Metric | Value |
|---|---|
| **Poems** | 13,828 |
| **Dictionary entries** | 33,640 |
| **Searchable verses** | 106,037 |
| **Test functions** | 128+ |

**Stack:** Swift · SwiftUI · CoreData · on-device NLP · privacy-first (no server, no telemetry)

→ [**trybayan.com**](https://trybayan.com)

---

### 💰 [FIML](https://kiarashplusplus.github.io/FIML/) — Financial Intelligence Meta-Layer

An AI-native MCP server for financial data aggregation with intelligent multi-provider orchestration and multilingual compliance guardrails. Open-source project demonstrating enterprise-grade AI architecture.

**32K+ lines of code · 1,403 automated tests · 100% pass rate**

**Stack:** Python · MCP Server · AI Orchestration · CI/CD

→ [Documentation](https://kiarashplusplus.github.io/FIML/) &nbsp;|&nbsp; [GitHub](https://github.com/kiarashplusplus/FIML)

---

### 🎤 [Aligna](https://www.align-a.com/) — Conversational AI Recruiter

Schedules and conducts voice interviews via LiveKit, transcribes with Azure OpenAI, and performs automated candidate-job matching with full observability.

**Stack:** Next.js · LiveKit · Azure OpenAI · PostgreSQL · Docker

→ [**align-a.com**](https://www.align-a.com/)

---

## Technical Identity

```text
Languages       TypeScript · Swift · Python · SQL
Infra           Cloudflare Workers · Durable Objects · R2 · D1 · KV · Queues
                Fastly Compute · E2B Sandboxes
Protocols       MCP (Model Context Protocol) · JSON-RPC 2.0 · WebSocket · OAuth 2.1
AI/ML           On-device NLP · LLM orchestration · AI safety (Llama Guard)
                Content moderation · Agent tooling
Frameworks      React · Next.js · Astro · Hono · SwiftUI · Vite
Security        Zero-knowledge encryption · Ed25519 signing · HMAC-SHA256
                SAML 2.0 · OIDC · Secret scanning · Path traversal protection
Dev Practice    Spec-Driven Development (SDD) · TDD · Immutable infrastructure
                Tamper-evident audit trails · Content-addressable storage
```

---

## What I'm Working On

- 🚀 Scaling [Undisk MCP](https://mcp.undisk.app) — SSO (SAML 2.0 + OIDC), Organizations, real-time audit webhook streaming for enterprise SIEM integration
- 🤝 [E2B partnership](https://mcp.undisk.app/e2b) — $20K compute grant establishing Undisk MCP + E2B as the de facto "Storage + Compute" architecture for AI agents
- 📱 Growing [Bayan](https://trybayan.com) — expanding the canonical corpus and refining on-device NLP for classical Persian poetry
- 📐 Evolving Spec-Driven Development tooling — building the workflow where specifications are the source of truth and code is a derived artifact

---

## Connect

| | |
|---|---|
| 🌐 **Portfolio** | [25x.codes](https://25x.codes) |
| 🔧 **Undisk MCP** | [mcp.undisk.app](https://mcp.undisk.app) |
| 📖 **Bayan** | [trybayan.com](https://trybayan.com) |
| 💼 **LinkedIn** | [linkedin.com/in/kiarashadl](https://linkedin.com/in/kiarashadl) |
| 🤖 **Ask my portfolio AI** | `curl https://25x.codes/.well-known/mcp.llmfeed.json` |

---

<sub>This profile is MCP-enabled. Point your AI agent at `https://25x.codes/.well-known/mcp.llmfeed.json` to query my projects, skills, and experience programmatically.</sub>
