<h1 align="center">Hi, I'm Deepak 👋</h1>

<p align="center">
  <b>Software engineer in Bengaluru, building LLM-agent infrastructure from first principles.</b>
</p>

<p align="center">
  <a href="https://github.com/mbsdeepak?tab=repositories"><img src="https://img.shields.io/badge/Projects-6+-1f6feb?style=flat-square" alt="Projects" /></a>
  <img src="https://img.shields.io/badge/Focus-LLM%20Agents-8957e5?style=flat-square" alt="Focus" />
  <img src="https://img.shields.io/badge/Language-Python-3572A5?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Bengaluru-🇮🇳-orange?style=flat-square" alt="Bengaluru" />
</p>

---

I'm an SDE building cost-intelligence and data-platform systems by day, and a full **LLM-agent stack** by night. Instead of reaching for a framework, I've been building each layer of the agent problem from scratch — small, readable, single-purpose libraries that compose into a complete platform.

## 🧩 The Agent Stack

Six independent libraries, each a few thousand readable lines of Python, that snap together into a working agent platform:

```mermaid
flowchart LR
    U["Task"] --> BH["🛡️ bulkhead<br/>resilient gateway"]
    BH --> CG["⚙️ cogs<br/>agent runtime"]
    LM["🧵 loom<br/>context engine"] --> CG
    CG --> SN["📡 sonar<br/>observability"]
    CG --> GT["🎯 gauntlet<br/>evals"]
    classDef box fill:#161b22,stroke:#30363d,color:#e6edf3;
    class U,BH,CG,LM,SN,GT box;
```

| Repo | What it is |
| :--- | :--- |
| **[cogs](https://github.com/mbsdeepak/cogs)** ⚙️ | A minimal but real **LLM agent runtime** — agent loop, typed tool protocol, provider abstraction, context management, permissions, and deterministic record/replay in ~1.5k lines. |
| **[loom](https://github.com/mbsdeepak/loom)** 🧵 | The **context-engineering layer** — chunking, embeddings, vector retrieval, history compaction, and token-budgeted context assembly. |
| **[bulkhead](https://github.com/mbsdeepak/bulkhead)** 🛡️ | A **resilient LLM gateway** — retries, circuit breaking, rate limiting, caching, failover, and cost governance in front of any provider. |
| **[gauntlet](https://github.com/mbsdeepak/gauntlet)** 🎯 | A rigorous **agentic tool-use eval set** — simulated tool environments, state/trajectory/LLM-judge grading, and pass@k with Wilson confidence intervals. |
| **[sonar](https://github.com/mbsdeepak/sonar)** 📡 | **Observability for agent runs** — an OpenTelemetry-style span tracer, cost/latency meters, and text/HTML trace timelines. |
| **[qwery](https://github.com/mbsdeepak/qwery)** 🔎 | A tiny **SQL query engine** over CSV & Parquet — hand-written tokenizer + recursive-descent parser feeding a Volcano-model executor (à la DuckDB). |

> Same philosophy throughout: **no magic, no heavy frameworks — just readable code that shows how the thing actually works.**

## 🛠️ Tech

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS_Bedrock-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Athena-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
</p>

## 📊 GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=mbsdeepak&show_icons=true&hide_border=true&theme=tokyonight&count_private=true" alt="stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mbsdeepak&layout=compact&hide_border=true&theme=tokyonight&langs_count=8" alt="top languages" />
</p>

## 🤝 Connect

<p>
  <a href="https://github.com/mbsdeepak"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <!-- Add your LinkedIn / blog / email badges here -->
</p>
