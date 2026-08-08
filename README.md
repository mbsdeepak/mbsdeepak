<div align="center">
  <img src="https://raw.githubusercontent.com/mbsdeepak/mbsdeepak/main/assets/hero.svg" alt="Bhargava Sai Deepak Mathukumalli — building LLM-agent infrastructure from first principles" width="820" />
</div>

<br/>

<p align="center">
  I build cloud cost-intelligence and data platforms professionally, and implement LLM-agent
  infrastructure from the ground up on my own time — one small, single-purpose library per hard
  problem, no framework in the way. The bias throughout: <b>build the thing to understand it</b> —
  minimal dependencies, code you can read end-to-end, behaviour you can inspect.
</p>

<br/>

## ⌁ &nbsp; An agent platform, built in layers

Each hard part of running an LLM agent, implemented as an independent library. They stand alone — and compose into a complete platform.

<div align="center">

```mermaid
flowchart LR
  T(["request"]) --> BH["🛡️ bulkhead<br/><i>gateway</i>"]
  BH --> CG["⚙️ cogs<br/><i>runtime</i>"]
  LM["🧵 loom<br/><i>context</i>"] --> CG
  CG --> SN["📡 sonar<br/><i>tracing</i>"]
  CG -. evals .-> GT["🎯 gauntlet"]
  classDef n fill:#161b22,stroke:#30363d,color:#e6edf3,rx:8,ry:8;
  class T,BH,CG,LM,SN,GT n;
```

</div>

| Project | What it solves | Notable internals |
| :-- | :-- | :-- |
| **[cogs](https://github.com/mbsdeepak/cogs)** | The agent runtime | Agent loop, typed tool protocol, provider abstraction, context management, permissions, and deterministic record/replay — in ~1.5k lines. |
| **[loom](https://github.com/mbsdeepak/loom)** | Context engineering | Chunking, embeddings, vector retrieval, history compaction, and token-budgeted context assembly. |
| **[bulkhead](https://github.com/mbsdeepak/bulkhead)** | Provider resilience | Retries, circuit breaking, rate limiting, caching, failover, and cost governance in front of any provider. |
| **[gauntlet](https://github.com/mbsdeepak/gauntlet)** | Agentic evaluation | Deterministic simulated tool environments, state/trajectory/LLM-judge grading, and pass@k with Wilson confidence intervals. |
| **[sonar](https://github.com/mbsdeepak/sonar)** | Run observability | OpenTelemetry-style span tracer, cost/latency meters, and text/HTML trace timelines. |
| **[qwery](https://github.com/mbsdeepak/qwery)** | SQL over raw files | Hand-written tokenizer + recursive-descent parser feeding a Volcano-model executor over CSV/Parquet — the design behind DuckDB, in pure Python. |

## ⌁ &nbsp; Currently

Cloud cost-intelligence — an LLM agent that answers cost questions over large-scale usage data, and the analytics pipelines behind it on Kubernetes.

<b>Reach for:</b> &nbsp; <code>Python</code> &nbsp; <code>Go</code> &nbsp; <code>C++</code> &nbsp; <code>AWS · Bedrock · Athena</code> &nbsp; <code>Kubernetes · Argo</code> &nbsp; <code>SQL</code>

<br/>

<p align="center">
  <code>$ contact</code> &nbsp;·&nbsp;
  <a href="https://linkedin.com/in/mbsdeepak"><b>LinkedIn</b></a> &nbsp;·&nbsp;
  <a href="mailto:mbsdeepak3@gmail.com"><b>mbsdeepak3@gmail.com</b></a>
</p>
