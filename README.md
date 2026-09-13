## Hi there 👋

<div align="center">

# Luis Navarro

### AI Systems · Backend Architecture · Full-Stack Product Engineering

Building production software around **LLMs, APIs, data, workflows, and real users**.

<img src="https://skillicons.dev/icons?i=python,ts,react,nextjs,nodejs,postgres,redis,docker,aws&perline=9" />

<br/>

`Python` · `FastAPI` · `TypeScript` · `Next.js` · `PostgreSQL` · `RAG` · `AI Agents` · `AWS`

</div>

---

## ⚡ What I Build

<table>
<tr>
<td width="50%" valign="top">

### 🧠 AI Systems

Production LLM applications that go beyond a prompt and an API call.

- RAG & semantic retrieval
- AI agents & tool calling
- Structured LLM outputs
- Document intelligence
- Evaluation & validation
- Human-in-the-loop workflows
- OpenAI · Claude · Gemini

</td>
<td width="50%" valign="top">

### ⚙️ Product & Backend

The application layer that keeps AI useful in production.

- REST APIs & backend services
- Async jobs & workflow state
- Authentication & authorization
- PostgreSQL / pgvector / Redis
- External system integrations
- React / Next.js applications
- AWS · Docker · CI/CD

</td>
</tr>
</table>

---

## 🏗️ Production Work

<details open>
<summary><strong>🏥 HealOS.ai — Healthcare AI Automation</strong></summary>

<br/>

Healthcare automation platform covering clinical documentation, insurance verification, prior authorization, patient communication, fax/referral processing, billing, and EHR connectivity.

**My work:** backend services, APIs, document pipelines, structured extraction, validation, background processing, workflow state, human review, and FHIR/EHR integration.

One recurring issue was that an LLM could return structurally valid data while still missing information required by the healthcare workflow. We kept model output separate from application state, validated required fields and conflicting values, and stopped uncertain cases for retry or staff review rather than allowing them to move downstream.

**Engineering areas:**  
`FastAPI` `PostgreSQL` `LLMs` `OCR` `FHIR` `Background Jobs` `Validation`

</details>

<br/>

<details>
<summary><strong>📈 LedgerLens — AI Financial Research</strong></summary>

<br/>

Financial research platform that combines company information, financial documents, retrieval, and LLM-assisted analysis.

**My work:** Next.js application development, FastAPI services, PostgreSQL/pgvector, document ingestion, vector retrieval, and LangGraph workflows.

Financial values and supporting evidence remained anchored to source data rather than being generated freely by the model. The LLM interpreted and explained retrieved information while the application preserved the documents and evidence behind the result.

**Engineering areas:**  
`Next.js` `FastAPI` `PostgreSQL` `pgvector` `RAG` `LangGraph`

</details>

<br/>

<details>
<summary><strong>🚛 GaugePro.io — Operations & Maintenance SaaS</strong></summary>

<br/>

Heavy-duty repair management software covering service orders, preventive maintenance, assets, diagnostics, parts inventory, communication, and reporting.

**My work:** backend services, APIs, scalable data models, workflow logic, and frontend application features.

The product contains several connected operational workflows, so changes to assets, service orders, maintenance records, or inventory need to remain consistent across related screens and reports. I worked on keeping those business rules in the application layer rather than duplicating them throughout the UI.

**Engineering areas:**  
`APIs` `Data Modeling` `React` `SaaS Workflows` `Reporting`

</details>

---

## 🧩 My Stack

### AI & LLM

<p>
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/Anthropic-191919?style=flat-square"/>
<img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square"/>
<img src="https://img.shields.io/badge/LlamaIndex-6C47FF?style=flat-square"/>
</p>

### Application

<img src="https://skillicons.dev/icons?i=python,fastapi,django,nodejs,ts,react,nextjs,vite" />

### Data & Infrastructure

<img src="https://skillicons.dev/icons?i=postgres,redis,mongodb,supabase,aws,docker,githubactions,vercel" />

---

## 🔍 How I Think About Production AI

```text
User request
     │
     ▼
Application / API
     │
     ├── Authentication & permissions
     ├── Business rules
     ├── Retrieval / tools
     │
     ▼
   LLM
     │
     ▼
Structured output
     │
     ├── Schema validation
     ├── Business validation
     ├── Confidence / evidence
     │
     ▼
Workflow decision
     │
     ├── Continue
     ├── Retry
     └── Human review
