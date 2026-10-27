### Aibu

Systems and infrastructure engineer working with **Rust**. Interested in deterministic execution runtimes, embedded storage engines, and reliability tooling for autonomous agents.

#### Current Work & Research Areas

- **Agent Execution Runtime (`systemone-mcp-core`)**: Low-latency UI interaction runtime, zero-copy DOM/XML delta compression, and confidence-gated state machines built on single-forward-pass evaluation primitives (`noul`, `choice`, `score`).
- **Transactional State & Storage (`agent-memory-rs`)**: Append-only WAL storage (`Bitcask` / `mmap`), `JournaledState` snapshot/revert semantics for isolated multi-agent branching, and SIMD-accelerated vector indexing.
- **Verification & Fault Injection (`agent-verify-gateway`)**: High-concurrency streaming proxies (`Tokio` / `Hyper` / `Tower`), multi-agent quorum verification pipelines, lock-free token budget circuit breakers, and chaos testing.

#### Active Repositories

- [**systemone-mcp-core**](https://github.com/wssab314/systemone-mcp-core) — Zero-copy UI context delta compressor and confidence-gated state machine in Rust.
- **agent-memory-rs** *(in progress)* — Snapshot-revertible embedded KV and vector storage engine for multi-agent state management.
- **agent-verify-gateway** *(planned)* — Streaming RPC/SSE router with quorum verification and fault injection.

#### Technical Stack

- **Languages**: Rust, Go, Python, TypeScript
- **Systems & Networking**: Tokio, Hyper, Tower, `memmap2`, `crossbeam`, `dashmap`
- **Profiling & Verification**: `cargo-flamegraph`, `samply`, `jemalloc`, `criterion.rs`, `proptest`
