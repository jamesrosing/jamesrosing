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

**heme** `private` - EHR for independent practices · monolith on InterSystems IRIS Native · TypeScript + React + Vite · custom design system, FHIR R4 layer in flight

**UDKS** - `private` - Unified Disease-Knowledge System · resolves any clinical code to cited reference knowledge · UMLS-CUI spine reconciled with Mondo · FHIR R4 terminology service · citation-faithful GraphRAG built last

**AEON** - Longevity intelligence platform · 400+ biomarkers · 30+ concurrent agents · multi-omics

**create-autoresearch** - Autonomous AI research loops for web apps · adapts [karpathy/autoresearch](https://github.com/karpathy/autoresearch) for webapp optimization · published on [npm](https://www.npmjs.com/package/create-autoresearch)

**indexer-ai** - Universal code indexer for AI assistants · published on [npm](https://www.npmjs.com/package/indexer-ai)

**FAL** - Omnichannel patient communication · Twilio + Zenoti integration

**LITMUS** - OpenAI verification protocol · fail-closed grounding layer where a generated claim acts only when it carries a warrant the gate can re-check against the domain's source of truth · public, early-stage · TypeScript

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
| **heme** `private` | EHR for 1-5 provider private practices - real IRIS Native persistence, monolith, TypeScript + React + Vite, custom design system, FHIR R4 layer in flight | - |
| **UDKS** `private` | Unified Disease-Knowledge System - resolves a clinical code to cited reference knowledge through a UMLS-CUI spine reconciled with Mondo, exposed as a FHIR R4 terminology service | - |
| **create-autoresearch** | Autonomous AI research loops for webapps - 9 optimization modes, auto-detects stack | [repo](https://github.com/jamesrosing/autoresearch) · [npm](https://www.npmjs.com/package/create-autoresearch) |
| **indexer-ai** | Universal code indexer - 3.6x faster with Worker Threads, 10K files in ~25s | [repo](https://github.com/tacit-code/indexer) · [npm](https://www.npmjs.com/package/indexer-ai) |
| **impression** | Design system extraction - Playwright, CIE ΔE 2000, multi-format output | [repo](https://github.com/jamesrosing/impression) |
| **zenoti-mcp-server** | MCP server for spa/wellness - AI-driven booking, billing, guests | [repo](https://github.com/tacit-code/zenoti-mcp-server) · [npm](https://www.npmjs.com/package/zenoti-mcp-server) |
| **zenoti-docs** | Zenoti API documentation mirror for offline / AI use | [repo](https://github.com/tacit-code/zenoti-docs) |
| **peptide** | Medical provider certification - searchable database, CME courses | [repo](https://github.com/jamesrosing/peptide) |
| **dashboard** | Real-time 3D multi-entity visualization - 1000+ updates/s at 60 fps | [repo](https://github.com/jamesrosing/dashboard) |
| **KEEL** `private` | AI-powered pre-med guidance - 9 advisor personas, vector matching | [repo](https://github.com/tacit-code/KEEL) |
| **AEON** `private` | Longevity intelligence - 400+ biomarkers, 30+ agents, multi-omics | - |
| **FAL** `private` | Omnichannel patient comms - Twilio, Zenoti, Messenger, SMS | [site](https://allure-md.com) |
| **SAIL** | Marine wind prediction - IoT sensors, time-series models | [repo](https://github.com/tacit-code/sail) · [live](https://sail-rouge.vercel.app/) |
| **frontend-quality-auditor** | Automated design-system QA - WCAG 2.1 AA, PRD validation | [repo](https://github.com/tacit-code/frontend-quality-auditor) |
| **deep-agents-ui** | Custom UI for deep agent workflows | [repo](https://github.com/tacit-code/deep-agents-ui) |
| **tebra-mcp-server** | MCP server for Tebra/Kareo practice management - 45 SOAP + FHIR clinical tools | [repo](https://github.com/jamesrosing/tebra-mcp-server) · [npm](https://www.npmjs.com/package/tebra-mcp-server) |
| **LITMUS** | OpenAI verification protocol - fail-closed grounding layer; a generated claim acts only when it carries a warrant the gate can re-check against the domain's source of truth, refusing by default otherwise | - |

---

<details>
<summary><strong>Project details ▸</strong></summary>

<br>

#### heme `private`
Electronic Health Record for Independent Practices

Monolithic EHR designed for 1-5 provider private practices. Real InterSystems IRIS Native persistence (not a Mongo-shaped mock), Express + TypeScript backend, React + Vite frontend, Lerna monorepo. Modules wired end-to-end against IRIS: auth, patients, scheduling, clinical notes/vitals/allergies/problems, audit, billing (charge / claim / payment with state machine), inbox, medications. FHIR R4 compliance layer and Bulk-FHIR interop in progress.

`TypeScript` `InterSystems IRIS Native` `Express` `React 19` `Vite 7` `Tailwind 3` `Lerna`

- Real IRIS Native driver via `@intersystems/intersystems-iris-native` (extracted at build time, not committed)
- Audit logging at the repository layer - every PHI read/write captured to a dedicated global
- Custom design system (`heme`) - three-anchor palette, no semantic colors, no pill shapes, status by icon + label + weight
- CI smoke job spins an IRIS container, vendors the driver, validates round-trip persistence on every PR

---

#### UDKS `private`
Unified Disease-Knowledge System

Keys narrative clinical reference content to a canonical medical code spine, so a diagnosis, medication, or lab code resolves to ranked pathophysiology, diagnosis, and treatment knowledge with crosswalks across every major coding system. The internal key is the UMLS CUI; ICD-10-CM, ICD-11, SNOMED, RxNorm, and LOINC are stored as projections, reconciled with Mondo for disease-class precision. Surfaced through a FHIR R4 terminology service and EHR-friendly delivery, with a citation-faithful GraphRAG layer built last. The release gate is citation fidelity: no clinical claim ships unless it traces to a verifiable source span.

`Python` `TypeScript` `PostgreSQL` `pgvector` `Apache AGE` `HAPI FHIR` `Mondo / SSSOM` `Claude Citations`

- UMLS-CUI spine with crosswalk projections across ICD-10-CM, ICD-11, SNOMED, RxNorm, LOINC, Mondo, HPO
- FHIR R4 terminology service (`$lookup` / `$translate` / `$expand` / `$validate-code`) on HAPI
- Open-core / hosted-premium split enforced by a CI redistribution guard and runtime row-level entitlement
- Citation-fidelity acceptance gate: every generated clinical claim carries an entailment-tested citation

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

#### create-autoresearch
Autonomous AI Research Loops for Web Applications

Adapts [karpathy/autoresearch](https://github.com/karpathy/autoresearch) for webapp optimization. An AI agent autonomously modifies your code, runs evaluation, keeps improvements, reverts failures, and repeats — overnight. Published on npm.

`TypeScript` `EJS` `Node.js CLI` `Lighthouse` `Vitest` `ESLint`

- 9 research modes: perf, quality, security, a11y, clean, wiring, styling, marketing, feature
- Auto-detects framework (Next.js, Nuxt, SvelteKit, Vite, Remix)
- Auto-detects integrations (Supabase, Prisma, Stripe, Clerk, shadcn)
- Configurable guardrails with HIPAA compliance support
- ~60-100 autonomous experiments per overnight session

-> [View Repository](https://github.com/jamesrosing/autoresearch) · [npm](https://www.npmjs.com/package/create-autoresearch)

---

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

-> [View Repository](https://github.com/tacit-code/zenoti-mcp-server) · [npm](https://www.npmjs.com/package/zenoti-mcp-server)

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

---

#### LITMUS
OpenAI Verification Protocol

A fail-closed grounding layer: a generated claim may act only when it carries a warrant the gate can re-check against the domain's source of truth, and the system refuses by default otherwise. Distinguishes weak referential warrants (a pointer to a source) from strong derivational warrants (re-running the underlying query, test, or computation), and routes the important-but-unverifiable case to a human with the evidence laid out. Architecture and principles are published; the first vertical, SMS delivery-truth and response attribution for FAL, is in implementation. Built vertical-first, the portable contract is extracted only once two real verticals share it.

`TypeScript`

- Fail-closed gate: refuses by default unless a claim carries a re-checkable warrant
- Referential vs derivational warrants - pointer to a source vs re-running the query/test/computation
- Important-but-unverifiable claims routed to a human with evidence laid out
- First vertical: SMS delivery-truth and response attribution for FAL
- Vertical-first; portable contract extracted only once two verticals share it

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
| **Published** | npm · [indexer-ai](https://www.npmjs.com/package/indexer-ai) · [create-autoresearch](https://www.npmjs.com/package/create-autoresearch) · [tebra-mcp-server](https://www.npmjs.com/package/tebra-mcp-server) · [zenoti-mcp-server](https://www.npmjs.com/package/zenoti-mcp-server) |

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
