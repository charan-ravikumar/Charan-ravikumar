<!--
  README.md — GitHub Profile
  Replace before publishing:
    - YOUR_GITHUB_USERNAME  → your GitHub username (used in stats/streak/typing-svg widgets)
    - PORTFOLIO_URL         → your portfolio site, or delete the badge if you don't have one
-->

<div align="center">

# R Charan

### GenAI Engineer · RAG Systems · Agentic AI · Databricks & Snowflake

Building production-grade retrieval and multi-agent systems — hybrid retrieval fusion, evaluation
harnesses that catch hallucination before it reaches a user, and deployments that go beyond
proof-of-concept into real, running platforms.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-charanravikumar-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/charanravikumar)
[![Email](https://img.shields.io/badge/Email-charanravikumar15%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:charanravikumar15@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-charan--ravikumar-181717?style=flat&logo=github&logoColor=white)](https://github.com/charan-ravikumar)

</div>

<br>

<!--
  ANIMATED TYPING BANNER (readme-typing-svg by DenverCoder1)
  Cycles through a short set of professional role statements.
-->
<div align="center">
  <a href="https://github.com/charan-ravikumar">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=2E75B6&center=true&vCenter=true&width=600&lines=GenAI+Engineer;RAG+%26+Hybrid+Retrieval+Systems;Agentic+AI+with+LangGraph;Evaluation+%26+Hallucination+Detection;Production+AI+on+Databricks+%2F+Snowflake" alt="Typing SVG" />
  </a>
</div>

<br>


## About Me

- GenAI Engineer at **Tredence Inc.** (Sept 2024 – Present), building RAG and agentic AI systems
  for enterprise clients.
- B.Tech, Metallurgical & Materials Engineering, **NIT Karnataka (Surathkal)**, 2020–2024.
- Core focus: **hybrid retrieval fusion** (BM25 + dense + RRF), **agentic orchestration** with
  LangGraph, and **evaluation/trust** — confidence scoring, hallucination detection, ablation
  studies.
- Shipped a GenAI solution to **production on the Snowflake Apps platform**, beyond its original
  proof-of-concept scope — a deployment signal, not just a demo.
- Industry exposure: **medical devices** (regulated document Q&A) and **medtech supply chain**
  (commercial root-cause analysis for inventory obsolescence).
- Certified: **Databricks Generative AI Engineer Associate**, **Microsoft Azure AI Engineer
  Associate (AI-102)**, **Databricks Machine Learning Associate**.
- Interested in evaluation-driven AI engineering — systems that are only trusted once they're
  measured, not just built.

---

## Tech Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)

**GenAI / LLMs**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat)
![OpenAI](https://img.shields.io/badge/Azure_OpenAI-GPT--4o-412991?style=flat&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat)

**Retrieval & Vector Search**

![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F00?style=flat)
![FAISS](https://img.shields.io/badge/FAISS-4267B2?style=flat)
![Databricks Vector Search](https://img.shields.io/badge/Databricks_Vector_Search-FF3621?style=flat&logo=databricks&logoColor=white)
![Snowflake Cortex](https://img.shields.io/badge/Snowflake_Cortex-29B5E8?style=flat&logo=snowflake&logoColor=white)

**Cloud & Data Platforms**

![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat&logo=snowflake&logoColor=white)
![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

**Backend & Observability**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)

**Data / ML**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)

</div>

---

## Featured Projects

### 1. Hybrid RAG Retrieval Ablation Study
**[github.com/charan-ravikumar/Advanced-Rag](https://github.com/charan-ravikumar/Advanced-Rag)**

A hybrid RAG pipeline (spaCy semantic chunking, BM25 + dense retrieval, RRF fusion, optional
CrossEncoder reranker) evaluated through a rigorous 4-config ablation study, shipped as a real
service — not just a notebook.

- **Stack:** Python, FastAPI, spaCy, ChromaDB Cloud, `rank_bm25`, sentence-transformers, RAGAS,
  Redis, Prometheus
- **Impact:** Improved Recall@5 by **43.6%** (0.188 → 0.270) while cutting P50 latency to **1.7s**.
  Isolated the actual source of the gain: RRF fusion alone, not BM25 in isolation.
- **Engineering challenge:** Designing four ablation configs as pure parameter variants (not code
  variants) to rule out implementation-difference confounds, then backing every claim with a
  custom evaluation harness (Recall@K, MRR, P50/P95/P99 latency) plus an optional RAGAS layer.

### 2. Multi-Agent AI Research Analyst
**[github.com/charan-ravikumar/Multi-Agent-AI-Research-Analyst](https://github.com/charan-ravikumar/Multi-Agent-AI-Research-Analyst)**

An autonomous LangGraph research system — planner, parallel research agents, a bounded
self-critique loop, and a human-in-the-loop approval checkpoint — that discloses contradictions
and gaps instead of hiding them.

- **Stack:** Python, LangGraph, Groq, Gemini, Redis, Streamlit
- **Impact:** Built an LLM-judged evaluation harness that caught the self-correction loop actively
  *degrading* faithfulness (93.3% → 39.1%); root-caused it to an ambiguous prompt, fixed it, and
  verified recovery to zero genuine hallucination.
- **Engineering challenge:** Proving the self-correction loop was structurally correct (bounded,
  terminating) was not enough — the eval harness was what proved it was actually harmful, then
  confirmed the fix worked. Verification over assumption, end to end.

---

## Professional Highlights

- **Production deployment beyond PoC scope** — delivered a Snowflake Cortex GenAI solution on the
  **Snowflake Apps platform**, where the original engagement called for a non-executing
  proof-of-concept.
- **Regulated-domain RAG** — designed retrieval, confidence scoring, and query routing for a
  medical-device document-intelligence platform (FDA / ISO 13485 / ISO 11608 context), where a
  confidently wrong answer is worse than no answer.
- **Enterprise-scale retrieval** — RAG corpus of **250+ enterprise documents** with a three-tier
  hybrid fusion architecture and a two-signal confidence-scoring engine (retrieval similarity +
  LLM-based claim grounding).
- **Agentic systems with real evaluation** — LangGraph multi-agent orchestration with bounded
  self-correction loops and human-in-the-loop checkpoints, validated with an LLM-judged evaluation
  harness rather than assumed to work.
- **Real-time computer vision at scale** — parallel multi-model inference pipeline cutting
  per-person latency **~8x** (~400ms → ~50ms), running at **~25 FPS on CPU-only hardware**.

---

## Current Focus

- Deepening evaluation methodology for agentic systems — moving beyond "does it run" to "does it
  actually help," the way the faithfulness regression in the Multi-Agent Research Analyst project
  was caught and fixed.
- Exploring GPU-backed reranking and lower-latency hybrid retrieval configurations.
- Strengthening statistical/EDA fundamentals to complement evaluation-methodology work.

---

## Open to Collaborate On

- Hybrid retrieval and RAG evaluation tooling
- Agentic workflows built on LangGraph with human-in-the-loop design
- Production-oriented GenAI systems (observability, caching, deployment — not just prototypes)

Feel free to open an issue or reach out directly.

---

## Certifications

- Databricks Certified Generative AI Engineer Associate
- Microsoft Certified: Azure AI Engineer Associate (AI-102)
- Databricks Certified Machine Learning Associate
  
---

## Connect 

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-charanravikumar-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/charanravikumar)
[![Email](https://img.shields.io/badge/Email-Reach_Out-D14836?style=flat&logo=gmail&logoColor=white)](mailto:charanravikumar@outlook.com)
<!-- [![Portfolio](https://img.shields.io/badge/Portfolio-Visit-2E75B6?style=flat&logo=googlechrome&logoColor=white)](PORTFOLIO_URL) -->

Bengaluru, India

<img src="https://komarev.com/ghpvc/?username=charan-ravikumar&style=flat&color=2E75B6" alt="Profile views" />

</div>
