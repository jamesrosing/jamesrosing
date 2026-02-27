<h1 align="center">James H. Rosing</h1>

<p align="center">
<strong>Plastic & Reconstructive Surgeon · AI Systems Architect</strong><br>
MD, FACS · Newport Beach, CA
</p>

<p align="center">
Board-certified plastic surgeon building production infrastructure that connects<br>
AI agents to real-world operations - healthcare, developer tooling, and IoT.
</p>

<p align="center">
<a href="https://scholar.google.com/citations?user=V3IzcHsAAAAJ">Google Scholar</a> ·
<a href="https://github.com/tacit-code">Tacit (Org)</a> ·
<a href="https://allure-md.com">Allure MD</a> ·
<a href="https://www.linkedin.com/in/allure-md-james-rosing/">LinkedIn</a> ·
<a href="mailto:jamesrosing@gmail.com">Email</a>
</p>

---

```
TypeScript · Python · Go · Next.js · React · Three.js · Tailwind
Node.js · PostgreSQL · Supabase · Redis · Docker · Vercel · Claude · OpenAI
```

---

### Currently Building

**AEON** - Longevity intelligence platform · 400+ biomarkers · 30+ concurrent agents · multi-omics

**indexer-ai** - Universal code indexer for AI assistants · published on [npm](https://www.npmjs.com/package/indexer-ai)

**FAL** - Omnichannel patient communication · Twilio + Zenoti integration

---

## Papers

| Paper | Description |
|:------|:------------|
| [Four-Loop Convergence](papers/four-loop-convergence/four-loop-convergence.md) | Iterative depth as a universal computational primitive - why feedback systems converge at ~4 iterations across neural computation, immunology, crystallography, and cognition |
| [The Other Side of the Room](papers/the-other-side-of-the-room/the-other-side-of-the-room.md) | Roommates, mental health leave, and the case for inclusive university policy - examining the evidence gap surrounding roommate impact when students return from psychiatric hospitalization |

---

## Projects

> Repos live across my personal account and [tacit-code](https://github.com/tacit-code) (my org).

| Project | What it does | |
|:--------|:-------------|:-:|
| **indexer-ai** | Universal code indexer - 3.6x faster with Worker Threads, 10K files in ~25s | [repo](https://github.com/tacit-code/indexer) · [npm](https://www.npmjs.com/package/indexer-ai) |
| **impression** | Design system extraction - Playwright, CIE ΔE 2000, multi-format output | [repo](https://github.com/jamesrosing/impression) |
| **zenoti-mcp-server** | MCP server for spa/wellness - AI-driven booking, billing, guests | [repo](https://github.com/tacit-code/zenoti-mcp-server) |
| **zenoti-docs** | Zenoti API documentation mirror for offline / AI use | [repo](https://github.com/tacit-code/zenoti-docs) |
| **peptide** | Medical provider certification - searchable database, CME courses | [repo](https://github.com/jamesrosing/peptide) |
| **dashboard** | Real-time 3D multi-entity visualization - 1000+ updates/s at 60 fps | [repo](https://github.com/jamesrosing/dashboard) |
| **KEEL** `private` | AI-powered pre-med guidance - 9 advisor personas, vector matching | [repo](https://github.com/tacit-code/KEEL) |
| **AEON** `private` | Longevity intelligence - 400+ biomarkers, 30+ agents, multi-omics | - |
| **FAL** `private` | Omnichannel patient comms - Twilio, Zenoti, Messenger, SMS | [site](https://allure-md.com) |
| **SAIL** | Marine wind prediction - IoT sensors, time-series models | [repo](https://github.com/tacit-code/sail) · [live](https://sail-rouge.vercel.app/) |
| **frontend-quality-auditor** | Automated design-system QA - WCAG 2.1 AA, PRD validation | [repo](https://github.com/tacit-code/frontend-quality-auditor) |
| **deep-agents-ui** | Custom UI for deep agent workflows | [repo](https://github.com/tacit-code/deep-agents-ui) |

---

<details>
<summary><strong>Project details ▸</strong></summary>

<br>

#### KEEL `private`
AI-Powered Pre-Med Guidance System

Multi-persona AI mentor synthesizing wisdom from nine distinct advisor perspectives into personalized counsel for pre-medical students.

`TypeScript` `Next.js 14` `FastAPI` `Claude API` `PostgreSQL` `pgvector`

- 9 advisor personas with dynamic weighting
- Multi-persona synthesis engine
- Opportunity matching with vector similarity
- Commitment tracking and accountability

-> [View Repository](https://github.com/tacit-code/KEEL)

---

#### Impression
Design System Extraction Plugin

Claude Code plugin that extracts design systems from live websites using Playwright, outputs structured JSON, and generates Tailwind configs, CSS variables, shadcn themes, and W3C tokens.

`Node.js` `Playwright` `CIE ΔE 2000` `WCAG Auditing`

- Live URL extraction via browser automation
- 8 pre-extracted references (Stripe, Notion, Linear, YouTube)
- Multi-format output (Tailwind, CSS vars, shadcn, W3C, Figma)
- Project comparison with gap analysis

-> [View Repository](https://github.com/jamesrosing/impression)

---

#### Peptide
Medical Provider Certification Platform

Comprehensive resource for medical providers seeking peptide therapy information, certification, and verified supplier connections.

`Next.js` `TypeScript` `Supabase` `Tailwind CSS`

- Searchable peptide database
- CME-accredited certification courses
- Verified supplier directory
- HIPAA-compliant professional forums

-> [View Repository](https://github.com/jamesrosing/peptide)

---

#### Dashboard
Real-time 3D Multi-Entity Visualization

High-performance monitoring system rendering 100+ entities at 60fps with near-zero latency control.

`Three.js` `React Three Fiber` `WebGL Instancing` `Web Workers` `WebSockets` `Redux` `Next.js 15`

- 1000+ updates/second throughput
- Worker thread spatial indexing
- LOD + frustum culling optimization
- Protocol Buffers serialization

-> [View Repository](https://github.com/jamesrosing/dashboard)

---

#### indexer-ai
Universal Code Indexer for AI Assistants

Enterprise-grade codebase indexer with parallel processing. Published on npm.

`TypeScript` `Worker Threads` `Tree-sitter` `AST Parsing` `Claude SDK`

- 3.6x faster with Worker Threads
- 10,000 files in ~25 seconds
- 40% memory reduction
- 9 languages supported

-> [View Repository](https://github.com/tacit-code/indexer) · [npm](https://www.npmjs.com/package/indexer-ai)

---

#### zenoti-mcp-server
MCP Server for Spa/Wellness Management

Model Context Protocol server enabling AI agents to manage Zenoti operations - appointments, guests, billing.

`TypeScript` `MCP Protocol` `REST API` `Zenoti API`

- 4-step service booking in single call
- Guest lifecycle management
- Invoice & payment processing
- Agent-optimized responses

-> [View Repository](https://github.com/tacit-code/zenoti-mcp-server)

---

#### AEON `private`
Longevity Intelligence Platform

Multi-agent AI system for longevity optimization targeting insurers to demonstrate reduced claims via wearables.

`TypeScript` `Python` `Multi-Agent Orchestration` `Real-time ETL`

- 400+ biomarker integration
- 30+ concurrent AI agents
- Multi-omics data pipelines
- HIPAA-compliant infrastructure

---

#### FAL `private`
Medical Practice Platform

Omnichannel patient communication system with practice management integration.

`Next.js` `Twilio` `Zenoti` `Supabase` `HIPAA`

- Facebook Messenger
- Google Business Messages
- SMS aggregation
- Zenoti booking sync

---

#### SAIL
Marine Wind Prediction

Real-time wind sensor and prediction model positioned 100m from shore.

`Python` `Time Series` `IoT` `Weather APIs`

- Sailing enthusiasts
- Marine businesses
- Race committees
- Harbor operations

-> [View Repository](https://github.com/tacit-code/sail) · [Live](https://sail-rouge.vercel.app/)

</details>

---

## Background

|  |  |
|:--|:--|
| **Education** | MD - Keck School of Medicine, USC (2004) |
| | BA Biological Sciences - University of Southern California (1997) |
| **Credentials** | MD, FACS |
| **Specialty** | Plastic & Reconstructive Surgery |
| **Practice** | [Allure MD](https://allure-md.com) - Newport Beach, CA |
| **Experience** | 14 years clinical |
| **Affiliations** | American Board of Plastic Surgery · ASPS · Allergan Partner (14+ yrs) |
| **Engineering** | Junior Developer -> AI Systems Architect |
| **Published** | npm · [indexer-ai](https://www.npmjs.com/package/indexer-ai) |

<p align="center">
<a href="James-Rosing-CV.pdf"><strong>View Full CV (PDF)</strong></a>
</p>

---

<p align="center">
<a href="https://github.com/jamesrosing">
<img src="https://github-readme-stats.vercel.app/api?username=jamesrosing&show_icons=true&theme=transparent&hide_border=true&title_color=ffffff&icon_color=888888&text_color=aaaaaa&ring_color=555555" height="160" alt="GitHub Stats"/>
</a>
<a href="https://github.com/jamesrosing">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jamesrosing&layout=compact&theme=transparent&hide_border=true&title_color=ffffff&text_color=aaaaaa&langs_count=8" height="160" alt="Top Languages"/>
</a>
</p>

---

<p align="center">
<sub>Newport Beach, CA · <a href="https://www.linkedin.com/in/allure-md-james-rosing/">LinkedIn</a> · <a href="https://alluremd.com">Allure MD</a> · <a href="mailto:jamesrosing@gmail.com">Email</a></sub>
</p>

