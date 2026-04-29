# Datt Goswami

Engineer building AI infrastructure, Rust LLM serving systems, and continual-learning tools for coding agents.

Currently building:

- [`cl-agent`](https://github.com/dattgoswami/cl-agent) — continual-learning substrate for coding agents
- **Ferrum** — agent platform: tooling, memory, evals, MCP, tracing, and cost infrastructure -
Docs: [Ferrum Stack](https://drive.google.com/file/d/15N13R1c0gWQDTTNzfVQruilHJWlRwneQ/view?usp=sharing) | [Ferrum Platform Poster](https://drive.google.com/file/d/1yD4BJmNPHm3lDecZRchCPDTh9vz-uBc9/view?usp=sharing)

---

## Featured Work

| Project | What it is | Why it matters |
|---|---|---|
| [`cl-agent`](https://github.com/dattgoswami/cl-agent) | Continual-learning substrate for coding agents | Episode capture, replay, skill distillation, SOAR-style search, and SFT export to Ollama — [paper](https://github.com/dattgoswami/cl-agent/blob/main/paper/cl_agent_paper_pub.pdf) |
| [`axon`](https://github.com/dattgoswami/axon) | Async Rust LLM inference server | Candle-based local inference with dynamic batching, SSE streaming, Metal/CUDA/CPU fallback, and TurboQuant 4-bit KV-cache compression (7× lossless, ~2K → ~14K context) |
| [`ferrum-mcp`](https://github.com/dattgoswami/ferrum-mcp) | Rust MCP server for AI agents | Typed agent access to crypto prices, DeFi yield/risk, Solana wallet state, and semantic memory over stdio/HTTP |
| [`forge-core`](https://github.com/dattgoswami/forge-core) | Framework-agnostic domain layer for agentic SWE systems | Shared tools, schemas, guardrails, Docker sandbox, and eval harness portable across LangGraph, OpenAI Agents SDK, CrewAI, Google ADK, and AWS Strands |
| [`ferrum-core`](https://github.com/dattgoswami/ferrum-core) | Shared Rust foundation for Ferrum services | Unified `FaError`/`FaResult` types, structured JSON logging, and OTLP tracing without HTTP-framework lock-in |
| [`ferrum-memory`](https://github.com/dattgoswami/ferrum-memory) | Agent memory + experience replay buffer | Qdrant hybrid retrieval, RL experience tuples, and dream-cycle consolidation for continual learning |

## Selected Projects

- [`ferrum-evals`](https://github.com/dattgoswami/ferrum-evals) — CL evaluation harness for agent platforms: tool-correctness, trajectory quality, and guardrails as a CI gate, plus BWT / FWT / Plasticity Index across task curricula
- [`forge-agent`](https://github.com/dattgoswami/forge-agent) — Continual-learning coding agent surface: wake/dream cycle, MCP-driven task execution, prioritized experience replay
- [`ferrum-agent`](https://github.com/dattgoswami/ferrum-agent) — Multi-agent orchestration runtime: planning, execution, review, memory, and human-approval flow in a single control plane
- [`ferrum-relay`](https://github.com/dattgoswami/ferrum-relay) — Async Rust task relay for AI agents: typed worker dispatch, bounded mpsc backpressure, Tower middleware over axum
- [`tokengate`](https://github.com/dattgoswami/tokengate) — LLM API metering and billing in Rust: DashMap-sharded usage tracking, Rayon-parallel invoice computation, per-API-key rate limiting
- [`taste-memory`](https://github.com/dattgoswami/taste-memory) — Human-tier preference, prompt-asset, and episodic memory service — the user-facing complement to `ferrum-memory`'s machine-tier replay buffer
- [`PersonalKB`](https://github.com/dattgoswami/PersonalKB) — Offline-first hybrid-RAG CLI (Ollama + BM42 sparse + Qdrant RRF) over personal technical libraries — grounded answers with citations, zero API cost
- [`SVM-L2-Optimistic-Rollup`](https://github.com/dattgoswami/SVM-L2-Optimistic-Rollup) — SVM-based Layer 2 optimistic rollup PoC: Agave 2.3.x off-chain execution, Solana L1 settlement, Celestia DA
- [`Continual-Intelligence`](https://github.com/dattgoswami/Continual-Intelligence) — 12-part research survey across continual learning, RL, reasoning, and world models

## Paper

- [Low-Level Wind Climatology Related to Potential Wind Compression](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=_pqlWmwAAAAJ&citation_for_view=_pqlWmwAAAAJ:9yKSN-GCB0IC)

## Writing

**[Continual Intelligence](https://github.com/dattgoswami/Continual-Intelligence)** — 12-part research survey across continual learning, RL, reasoning, and world models.

**Production AI & agent systems**
- [Context Engineering: The Real Work Behind Production AI Systems](https://datt.substack.com/p/context-engineering-the-real-work)
- [Building AI That Actually Ships: An Engineer's Field Guide](https://open.substack.com/pub/datt/p/building-ai-that-actually-ships-an)
- [The Agent Framework Wars Are Already Over](https://datt.substack.com/p/the-agent-framework-wars-are-already)
- [The State and Future of Agentic AI](https://datt.substack.com/p/the-state-and-future-of-agentic-ai)

**Rust LLM inference & MCP**
- [TurboQuant in Rust: Provably Near-Optimal KV-Cache Compression](https://medium.com/@dattgoswami/turboquant-in-rust-provably-near-optimal-kv-cache-compression-for-llm-inference-servers-fb59f15c6216)
- [Building ferrum-mcp: A Production-Grade Rust MCP Server](https://medium.com/@dattgoswami/building-ferrum-mcp-a-production-grade-rust-mcp-server-for-ai-agents-in-crypto-and-defi-bba845dd14da)
- [MCP Patterns for DeFi Agents in Rust](https://medium.com/@dattgoswami/mcp-patterns-for-defi-agents-in-rust-931cec1cb6f8)

**Reasoning & continual learning**
- [Beyond Thinking Longer: How to Teach Language Models to Actually Explore](https://medium.com/@dattgoswami/beyond-thinking-longer-how-to-teach-language-models-to-actually-explore-3ae3297ee71f)
- [While We Wait for Continual Learning to Get Us to World Models, Program Synthesis Is the Dark Horse](https://open.substack.com/pub/datt/p/while-we-wait-for-continual-learning)

**Systems & blockchain**
- [Building an SVM Layer 2: Wiring Agave's TransactionBatchProcessor Into an Optimistic Rollup](https://medium.com/@dattgoswami/building-an-svm-layer-2-how-i-wired-agaves-transactionbatchprocessor-into-an-optimistic-rollup-042227042b48)
- [NASA's Lessons from 60y of Software Engineering- When Code Must Not Fail: Engineering for Mission-Critical Systems](https://datt.substack.com/p/when-code-must-not-fail-engineering)

## Stack

- **Rust & systems** — Tokio, DashMap, Candle (HuggingFace), axum, tower, serde, tracing/OTLP, async concurrency, KV-cache quantization, native Solana SVM
- **AI/ML** — LLM serving (batching, SSE, fallback), RAG, MCP, A2A, fine-tuning (QLoRA), RL (PPO/DPO/GRPO/SAC), LangGraph, PyTorch, Pinecone, W&B
- **Distributed infra** — AWS (Lambda, S3, DynamoDB, SQS/SNS, EventBridge, RDS), GCP, Docker, Kubernetes, Helm, Terraform, Kafka, Postgres, Redis
- **Languages** — Rust, Python, TypeScript, Java, Go, SQL

## Focus

- Coding-agent memory, replay, evaluation, and continual improvement
- Rust LLM inference and async backend systems
- MCP servers and typed agent tooling
- RAG, hybrid retrieval, and production AI systems

## Connect

- LinkedIn — [linkedin.com/in/dattgoswami](https://www.linkedin.com/in/dattgoswami)
- Substack — [datt.substack.com](https://datt.substack.com)
- Medium — [medium.com/@dattgoswami](https://medium.com/@dattgoswami)
- X — [@dattgoswami](https://x.com/dattgoswami)
- Email — dattgoswami@gmail.com
