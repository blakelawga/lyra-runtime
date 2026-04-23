<p align="center">
  <img width="400" alt="Lyra Logo" src="https://raw.githubusercontent.com/blakelawga/lyra-runtime/main/lyra-syt.png">
</p>

<h1 align="center"> Lyra-Core v2.1</h1>
<p align="center"><strong>High-throughput deterministic truth synthesis for Kalshi.</strong></p>
 
<p align="center">
  A distributed, low-latency execution layer for autonomous event-settlement and Bayesian truth-verification in regulated prediction markets.
</p>
 
---   
 
## Overview 
 
**Lyra** is a specialized, local-first settlement engine designed for the **Kalshi** ecosystem. It is engineered for developers who require sub-millisecond data triangulation and deterministic market resolution without the overhead of centralized oracular consensus.

Instead of relying on singular, fallible API endpoints, Lyra utilizes a **State-Space Search** model to map real-world entropy into binary finality ($S \to \{0, 1\}$). It collapses the infrastructure burden of event verification into a lightweight, high-performance runtime optimized for cold-start investigation and zero-trust auditability.

---

## On-Chain Verification

To ensure settlement integrity, Lyra implements an on-chain verification layer. Every decision is cryptographically attested to by a decentralized validator set, ensuring that the "Truth" synthesized off-chain is immutable and verifiable on-chain.



### Active Verifiers:
* **Verifier 1:** `BH7asDZbKkTmT3UWiNfmMVRgQEEpXoVThGPmQfgWwDhg`
* **Verifier 2:** `8M9BwRgSbVXmk843XDCgztkGgCotLUpkaW6qovZhk1QF`

Lyra generates **Zero-Knowledge Proofs (zk-SNARKs)** of its data retrieval and Bayesian synthesis, which are then validated by the above addresses before the final market resolution is pushed to the exchange.

---

## System Overview

Lyra acts as a compact, concurrent runtime for truth-seeking agents. It reduces the operational complexity of the broader oracle stack by condensing investigation, synthesis, and cryptographic signing into a single, performance-tuned environment.

The project emphasizes:

- **Non-Blocking I/O** utilizing `io_uring` for massive parallel data ingestion.
- **On-Chain Attestation** providing a transparent audit trail for all settled contracts.
- **LLM-Augmented Reasoning** for parsing complex legislative or regulatory text.
- **Minimal Operational Footprint** compared to full cloud-based oracle networks.

---

## Key Features

- **Deterministic Logic Engine** Uses Z3 SMT solvers to ensure settlement decisions strictly adhere to contract invariants.
- **Recursive Source Validation (RSV)** Eliminates single-point-of-failure by cross-referencing $N$ independent data streams.
- **High-Concurrency Ingress** Optimized Rust-based ingestors for real-time WebSocket and gRPC feed processing.
- **Explainable Evidence Bundles** Generates immutable, cryptographically signed snapshots of the data state at $t_0$.
- **Zero-Trust Finality** Integrated on-chain verification ensures that no single entity can manipulate the settlement outcome.

---

## Technology Stack

- **Rust** Core runtime implemented for memory safety and zero-cost abstractions.
- **Solana/SVM** High-speed on-chain verification layer for settlement attestations.
- **vLLM / TensorRT** Local inference engine for high-speed contextual reasoning.
- **NATS JetStream** Lightweight, distributed messaging for ultra-low latency.

---

## Quick Start

### 1. Clone the repository

```bash
git clone [https://github.com/kalshi-labs/lyra.git](https://github.com/kalshi-labs/lyra.git)
cd lyra
## Quick Start

### 1. Clone the repository

```bash
git clone [https://github.com/kalshi-labs/lyra.git](https://github.com/kalshi-labs/lyra.git)
cd lyra

## [verification]verifiers 
    = ["BH7asDZbKkTmT3UWiNfmMVRgQEEpXoVThGPmQfgWwDhg",
    "8M9BwRgSbVXmk843XDCgztkGgCotLUpkaW6qovZhk1QF"]
    cargo build --release --features="cuda_accel"
    ./target/release/lyra --contract-id "WILL-FED-HIKE-MAY" --live

## Quick Start

### 1. Clone the repository

```bash
git clone [https://github.com/kalshi-labs/lyra.git](https://github.com/kalshi-labs/lyra.git)
cd lyra
