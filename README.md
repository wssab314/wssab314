<div align="center">

# Hi there, I'm Aibu ⚡

### **AI Agent Systems & High-Performance Rust Engineer**

*“Don't Trust, Verify — Building database-grade runtime, transactional memory, and zero-trust verification infrastructure for autonomous AI Agents in pure Rust.”*

<p align="center">
  <img src="https://img.shields.io/badge/Focus-AI_Agent_Systems_Engineering-6366f1?style=for-the-badge&logo=rust&logoColor=white" alt="Focus" />
  <img src="https://img.shields.io/badge/Runtime-Rust_1.95_%2B_Tokio-dea584?style=for-the-badge&logo=rust&logoColor=black" alt="Rust" />
  <img src="https://img.shields.io/badge/Architecture-System--1_MCP_%26_Shared_Memory-10b981?style=for-the-badge" alt="MCP" />
</p>

</div>

---

### 🧭 Engineering Philosophy: The 5 Systems Primitives for AI Agents

Modern AI Agents are no longer simple prompt workflows — their engineering complexity rivals a **browser engine** or an **embedded database**. My work bridges battle-tested **high-frequency systems primitives** with **next-generation Agent infrastructure**:

| Systems Primitive | Origin in High-Frequency / Distributed Systems | Application in Hardcore AI Agent Engineering |
| :--- | :--- | :--- |
| **1. Zero-Trust Verification** | Byzantine Fault Tolerance (BFT) & Quorum Voting | **Group Evolution & Verify Gates**: Treat every LLM output as untrusted; gate actions via `<30ms` System-1 primitives (`noul` / `score`) & deterministic sandboxes. |
| **2. Transactional Memory** | Append-Only WAL, `mmap` & `JournaledState` Revert | **Revertible Shared Memory**: Enable 100+ sub-agents to `fork()` isolated memory branches and `revert(checkpoint)` failed explorations in `<10μs`. |
| **3. Delta Context Compression** | OrderBook Snapshot + Incremental Delta Streams | **96% Token Dehydration**: Zero-copy DOM/XML pruning + frame-to-frame tree diffing (`UiDeltaPatch`) to transmit only mutated UI/code nodes. |
| **4. Fast/Slow Path Split** | Sub-millisecond Fast-Path Reflex & Circuit Breakers | **System-1 UI Skills Runtime**: Offload 90% of routine GUI micro-actions from slow System-2 LLMs (`3.5s`) to local single-forward-pass models (`28ms`). |
| **5. Deterministic Guardrails** | Pre-Trade Risk Firewalls & Chaos Fault Injection | **Token Circuit Breakers & Chaos Testing**: Lock-free `AtomicU64` budget breakers and stream fault injectors to guarantee production survivability. |

---

### 🚀 Flagship Open-Source Suite

| Repository | Architecture Track | Core Rust Primitives | Status |
| :--- | :--- | :--- | :--- |
| ⚡ **[`systemone-mcp-core`](https://github.com/wssab314/systemone-mcp-core)** | **UI Skills & Delta Context Compression MCP Engine**<br/>Zero-copy SoM parser, OrderBook-style UI tree diffing (`-96%` tokens), and `/v1/systemone` (`noul`·`choice`·`score`) confidence gate. | `&'a str` Zero-Copy · `quick-xml` · `imageproc` · `serde` · FSM | ![Active](https://img.shields.io/badge/Status-Active_Development-22c55e?style=flat-square) |
| 🧠 **`agent-memory-rs`** | **Transactional Shared Memory & SIMD Vector Engine**<br/>Embedded single-file agent memory with `checkpoint()`/`revert()` rollback, Copy-on-Write multi-agent branching, and `ARM NEON SIMD` HNSW search. | `Bitcask WAL` · `memmap2` · `Cow` · `DashMap` · `NEON SIMD` · `SQ8` | ![Architecture](https://img.shields.io/badge/Phase-Storage_%26_Journal_Engine-6366f1?style=flat-square) |
| 🛡️ **`agent-verify-gateway`** | **Group Evolution Verifier & Chaos Gateway**<br/>Zero-copy SSE streaming router, multi-agent Quorum verification pipeline, lock-free Token budget circuit breaker, and chaos fault injector. | `Tokio` · `Hyper` · `Tower` · `AtomicU64` · `arc-swap` · `HdrHistogram` | ![Planned](https://img.shields.io/badge/Phase-Spec_%26_Design-f59e0b?style=flat-square) |

---

### 🛠️ Systems & Profiling Toolchain

<p align="left">
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" />
  <img src="https://img.shields.io/badge/Tokio_Async-1e293b?style=flat-square&logo=rust&logoColor=dea584" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux_%26_macOS_ARM64-FCC624?style=flat-square&logo=apple&logoColor=black" />
  <img src="https://img.shields.io/badge/SIMD_(ARM_NEON_%2F_AVX2)-0f172a?style=flat-square" />
  <img src="https://img.shields.io/badge/cargo--flamegraph-ef4444?style=flat-square" />
  <img src="https://img.shields.io/badge/jemalloc_%26_samply-8b5cf6?style=flat-square" />
  <img src="https://img.shields.io/badge/criterion.rs-06b6d4?style=flat-square" />
</p>
