# Hi, I'm Youngpil 👋

**Senior DevOps / MLOps Engineer | AI Infrastructure · GPU Platforms · Kubernetes · Linux Systems**

I build infrastructure where **GPU compute, high-performance networking, Kubernetes, storage, and ML workloads** meet.

My current focus is **AI Factory engineering** — designing reproducible GPU infrastructure, validating cluster networking, operating container platforms, diagnosing systems-level failures, and building reliable paths from model development to training and inference.

I enjoy turning infrastructure requirements into **deployable architectures, observable systems, automated validation, and practical developer platforms**.

## ⚡ AI Infrastructure Focus

* **GPU Platforms** — NVIDIA GPUs, CUDA, GPU workloads, DeepStream, DCGM, containerized training and inference
* **AI Cluster Networking** — InfiniBand, RDMA/RoCE, Ethernet, Clos fabrics, eBGP/ECMP, NetBox, Containerlab
* **Kubernetes Platforms** — Kubernetes, CRI/CNI, Cilium/Calico, GPU workloads, Helm, GitOps
* **Linux Reliability** — eBPF, cgroups, memory/OOM analysis, kernel crash diagnostics, observability
* **MLOps** — training/inference pipelines, model lifecycle, evaluation gates, lineage, W&B/MLflow
* **Infrastructure Automation** — AWS, Terraform, Ansible, GitHub Actions, CI/CD

---

## 🏭 AI Factory / GPU Infrastructure

### [AI Factory Network Twin](https://github.com/restack/ai-factory-network-twin)

**NetBox-driven AI cluster network digital twin and validation lab.**

Models a dual-plane L3 Clos fabric with FRR and Linux GPU endpoints, using **eBGP, ECMP, VRFs, deterministic topology generation, runtime verification, and reversible failure injection**.

The goal is to treat AI cluster networking as executable infrastructure: define intent, validate invariants, compile the fabric, deploy it, inject failures, and collect machine-readable evidence.

`NetBox` · `Containerlab` · `FRR` · `SR Linux` · `BGP` · `ECMP` · `Clos` · `Batfish`

---

### [ghostmem](https://github.com/ziwon/ghostmem)

**Rust + eBPF memory diagnostics for GPU and ML workloads.**

A Linux diagnostic TUI that identifies `/dev/shm` and `memfd` memory invisible to normal process RSS monitoring but still accounted for by cgroups and capable of triggering OOM kills.

Tracks shared-memory lifecycle, orphaned segments, cgroup pressure, allocation stacks, and optional **CUDA pinned/device memory** without requiring application changes or restarts.

`Rust` · `eBPF` · `libbpf` · `cgroups` · `CUDA` · `Linux` · `PyTorch`

---

### [VRS — Video Reasoning System](https://github.com/ziwon/vrs)

**GPU-oriented video reasoning platform built around perception → VLM verification.**

A VSS-inspired two-stage architecture where a fast perception pipeline generates candidate events and a slower VLM verifier evaluates visual evidence and policy context.

Designed around production-shaped boundaries including **NVIDIA DeepStream 8, GPU workers, Kubernetes/Helm, FastAPI, Redis Streams, S3-compatible storage, and multi-stream inference**.

The deployment model progresses from Docker Compose to single-GPU edge Kubernetes and multi-node clusters while preserving common runtime contracts.

`NVIDIA DeepStream` · `CUDA` · `Kubernetes` · `Helm` · `VLM` · `FastAPI` · `Redis`

---

### [AI Data Center Systems](https://adcs.restack.tech/)

**A living knowledge system for AI Factory infrastructure.**

An engineering wiki connecting the major layers of modern AI infrastructure:

**Network → GPU → Storage → Distributed Training → Inference → MLOps → Systems Performance**

Topics include **RDMA, InfiniBand, RoCE, Clos fabrics, CUDA architecture, GPU profiling, distributed training, KV cache, AI storage pipelines, model lifecycle, and systems performance engineering**.

The web platform adds AI-powered Q&A and interactive 2D/3D knowledge graphs over the engineering notes.

[Explore ADCS →](https://adcs.restack.tech/)

---

### [CrashShoot](https://github.com/ziwon/crashshoot)

**Evidence-driven Linux kernel postmortem tooling for production infrastructure.**

A Go-based operational layer around Linux `vmcore` analysis that validates crash artifacts and symbols before performing bounded analysis.

Produces reproducible, evidence-linked postmortem reports while integrating with tools such as `crash`, `drgn`, `gdb`, and `makedumpfile`.

Useful for diagnosing failures below the container and Kubernetes layers when infrastructure problems become kernel problems.

`Go` · `Linux Kernel` · `vmcore` · `crash` · `drgn` · `gdb`

---

## 🤖 ML Platforms / Production ML

### [Vision MLOps Reference](https://github.com/ziwon/vision-mlops)

A production-shaped computer vision lifecycle reference covering:

**raw data → annotation → dataset contracts → training → golden evaluation → promotion gates → model bundle → ONNX → inference → drift monitoring**

Built around MobileNetV4 + FCOS with optional SAM-assisted labeling and explicit control-plane/data-plane contracts.

`PyTorch` · `Computer Vision` · `MLOps` · `ONNX` · `CVAT` · `W&B`

---

### [CV False Positive Mining Lab](https://github.com/ziwon/cp-fp-mining-lab)

An active-learning workflow that converts production CV false positives into reviewed and versioned **hard-negative datasets and retraining signals**.

The pipeline combines embedding extraction, clustering, uncertainty/diversity ranking, human review, dataset lineage, retraining, evaluation, and promotion gates.

`YOLO` · `CLIP` · `UMAP` · `HDBSCAN` · `Label Studio` · `W&B`

---

### [RAG Adapt Lab](https://github.com/ziwon/rag-adapt-lab)

A reproducible GPU research harness for answering:

> When is plain RAG enough, and when does domain adaptation actually add measurable value?

Compares **Base, RAG, SFT + RAG, and RAFT + RAG** under common datasets, retrieval pipelines, evaluation protocols, and hardware constraints.

Designed for local and self-hosted experiments on commodity NVIDIA GPUs with explicit **quality / latency / VRAM trade-offs**.

`NVIDIA GPU` · `QLoRA` · `RAG` · `RAFT` · `W&B` · `LLM Evaluation`

---

## 🧩 Infrastructure / Developer Platforms

### [FlareGraph](https://github.com/ziwon/FlareGraph)

**Cloudflare-native LLM knowledge graph and agentic retrieval platform.**

Turns an Obsidian/Markdown knowledge base into an agent-accessible backend using R2, D1/FTS5, Vectorize embeddings, hybrid retrieval, knowledge graphs, REST APIs, and MCP.

`Cloudflare Workers` · `R2` · `D1` · `Vectorize` · `MCP` · `TypeScript`

---

### [Restack Actions](https://github.com/restack/actions)

Reusable GitHub Actions and repository automation, including Kubernetes manifest updates and local-LLM-powered repository analysis and modification.

`GitHub Actions` · `Kubernetes` · `GitHub Apps` · `CI/CD`

---

### [SpeakLoop](https://speak-loop.pages.dev/)

A speaking-first AI English coach for software engineers working in global teams, with real-time Gemini Live conversations, structured feedback, authentication, and usage quotas.

[Try SpeakLoop →](https://speak-loop.pages.dev/)

---

## 🔬 Other Projects

* **[Kernel Lens](https://kernel-lens.pages.dev/)** — Interactive exploration of Linux kernel and low-level systems concepts
* **[CapEx Lens](https://capex-lens.pages.dev/)** — Evidence-first dashboard tracking AI infrastructure investment momentum and hyperscaler monetization
* **[AKBO](https://akbo.pages.dev/)** — Web product experiment

---

## 🧠 How I Think About AI Infrastructure

I see an AI cluster as **one distributed system**, not a collection of independent GPU servers.

Reliable AI infrastructure requires the entire path to work together:

```text
GPU Compute
    ↕
Compute Fabric
    ↕
Storage / Data Path
    ↕
Kubernetes / Workload Scheduling
    ↕
Training & Inference Runtime
    ↕
Observability / Validation / Failure Analysis
```

That means understanding not only whether a workload runs, but **why it performs the way it does, how it fails, and how the platform behaves when components disappear under load**.

I prefer infrastructure that can be:

**defined → reproduced → validated → observed → broken intentionally → diagnosed → improved**

---

## 🌱 Currently Deepening

* NVIDIA AI Factory architectures
* GPU cluster operations and validation
* InfiniBand / Ethernet / RDMA / RoCE
* NCCL and distributed GPU communication
* Kubernetes GPU orchestration
* NVIDIA GPU / Network Operator ecosystem
* AI workload storage and data paths
* Distributed training and high-throughput inference
* GPU and Linux systems performance engineering

---

> **Building AI infrastructure from the kernel to the cluster — and from the cluster to the model.**
