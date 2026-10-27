<div align="center">

# Hi there, I'm Aibu ⚡

### **AI Agent Systems & High-Performance Rust Engineer**
#### **AI Agent 系统工程与高性能 Rust 基础设施研发**

*“Don't Trust, Verify — Building database-grade runtime, transactional memory, and zero-trust verification infrastructure for autonomous AI Agents in pure Rust.”*  
*“零信任，强验证 —— 用纯正 Rust 构建数据库级 AI Agent 极速运行时、可回滚共享记忆库与混沌验证网关。”*

<p align="center">
  <img src="https://img.shields.io/badge/Focus-AI_Agent_Systems_Engineering-6366f1?style=for-the-badge&logo=rust&logoColor=white" alt="Focus" />
  <img src="https://img.shields.io/badge/Runtime-Rust_1.95_%2B_Tokio-dea584?style=for-the-badge&logo=rust&logoColor=black" alt="Rust" />
  <img src="https://img.shields.io/badge/Architecture-System--1_MCP_%26_Shared_Memory-10b981?style=for-the-badge" alt="MCP" />
</p>

</div>

---

### 🧭 Engineering Philosophy · 核心工程理念：AI Agent 的五大系统级原语

Modern AI Agents are no longer simple prompt workflows — their engineering complexity rivals a **browser engine** or an **embedded database**. My work bridges battle-tested **high-frequency distributed systems primitives** with **next-generation Agent infrastructure**:  
现代 AI Agent 早已不再是简单的 Prompt 拼接，其系统工程复杂度堪比**小型浏览器引擎**或**嵌入式数据库**。我致力于将经过极端高并发检验的**底层系统原语**降维注入到下一代 **AI Agent 核心基础设施**中：

| Systems Primitive<br/>底层系统原语 | Origin in High-Frequency Systems<br/>高频/分布式系统本源 | Application in Hardcore AI Agent Engineering<br/>在硬核 AI Agent 系统工程中的落地形态 |
| :--- | :--- | :--- |
| **1. Zero-Trust Verification**<br/>**零信任交叉验证** | Byzantine Fault Tolerance (BFT) & Quorum Voting<br/>拜占庭容错投票与状态校验 | **Group Evolution & Verify Gates (多智能体交叉验证门控)**<br/>Treat every LLM output as untrusted; gate actions via `<30ms` System-1 primitives (`noul` / `score`) & deterministic sandboxes.<br/>默认单次模型输出不可信（必有幻觉），通过 30ms 端侧小模型原语与确定性沙盒验证通过后才放行。 |
| **2. Transactional Memory**<br/>**可回滚事务型记忆** | Append-Only WAL, `mmap` & `JournaledState` Revert<br/>预写日志与状态快照原子回滚 | **Revertible Shared Memory (支持分支与回滚的共享记忆库)**<br/>Enable 100+ sub-agents to `fork()` isolated memory branches and `revert(checkpoint)` failed explorations in `<10μs`.<br/>支持百个子 Agent 并发 `fork` 独立记忆分支探索，走入死胡同时 `<10μs` 瞬间回滚脏状态，验证通过后原子合并。 |
| **3. Delta Context Compression**<br/>**增量差分上下文压缩** | OrderBook Snapshot + Incremental Delta Streams<br/>高频盘口快照与增量差分流 | **96% Token Dehydration (毫秒级视图树脱水与差分压缩)**<br/>Zero-copy DOM/XML pruning + frame-to-frame tree diffing (`UiDeltaPatch`) to transmit only mutated UI/code nodes.<br/>基于零拷贝切片剥离 95% 冗余标签，并对比前后两帧界面树，仅向 Agent 发送发生变化的元素增量。 |
| **4. Fast/Slow Path Split**<br/>**快慢路径分离与熔断** | Sub-ms Fast-Path Reflex & Circuit Breakers<br/>微秒级热路径反射与风控熔断 | **System-1 UI Skills Runtime (30ms 极速 UI 技能执行核)**<br/>Offload 90% of routine GUI micro-actions from slow System-2 LLMs (`3.5s`) to local single-forward-pass models (`28ms`).<br/>将 90% 高频常规 UI 操作卸载至端侧单次前向传播小模型（28ms），连续 3 步无进展立即触发防死循环熔断。 |
| **5. Deterministic Guardrails**<br/>**确定性安全护栏与混沌工程** | Pre-Trade Risk Firewalls & Chaos Fault Injection<br/>前置风控防火墙与混沌故障注入 | **Token Circuit Breakers & Chaos Testing (无锁预算熔断与混沌评测)**<br/>Lock-free `AtomicU64` budget breakers and stream fault injectors to guarantee production survivability.<br/>基于 `AtomicU64` 实现微秒级无锁 Token 预算熔断器，并注入断流/弹窗故障量化评测 Agent 生产存活率。 |

---

### 🚀 Flagship Open-Source Suite · 三大核心开源项目矩阵

| Repository · 开源仓库 | Architecture Track · 架构定位与核心特性 | Core Rust Primitives · 核心技术栈 | Status · 状态 |
| :--- | :--- | :--- | :--- |
| ⚡ **[`systemone-mcp-core`](https://github.com/wssab314/systemone-mcp-core)** | **UI Skills & Delta Context Compression MCP Engine**<br/>**极速 UI Skills 与增量上下文压缩 MCP 引擎**<br/>Zero-copy SoM parser, OrderBook-style UI tree diffing (`-96%` tokens), and `/v1/systemone` (`noul`·`choice`·`score`) confidence gate. | `&'a str` Zero-Copy · `quick-xml` · `imageproc` · `serde` · FSM | ![Active](https://img.shields.io/badge/Status-Active_Dev-22c55e?style=flat-square) |
| 🧠 **`agent-memory-rs`** | **Transactional Shared Memory & SIMD Vector Engine**<br/>**事务型可回滚多智能体共享记忆与 SIMD 向量库**<br/>Embedded single-file agent memory with `checkpoint()`/`revert()` rollback, Copy-on-Write branching, and `ARM NEON SIMD` HNSW search. | `Bitcask WAL` · `memmap2` · `Cow` · `DashMap` · `NEON SIMD` · `SQ8` | ![Architecture](https://img.shields.io/badge/Phase-Storage_Engine-6366f1?style=flat-square) |
| 🛡️ **`agent-verify-gateway`** | **Group Evolution Verifier & Chaos Gateway**<br/>**多智能体交叉验证、无锁 Token 熔断与混沌工程网关**<br/>Zero-copy SSE streaming router, multi-agent Quorum verification pipeline, lock-free Token circuit breaker, and chaos fault injector. | `Tokio` · `Hyper` · `Tower` · `AtomicU64` · `arc-swap` · `HdrHistogram` | ![Planned](https://img.shields.io/badge/Phase-Spec_%26_Design-f59e0b?style=flat-square) |

---

### 🛠️ Systems & Profiling Toolchain · 系统研发与性能剖析工具链

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
