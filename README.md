# 🚀 Dynomite-Project

![GitHub Repo stars](https://img.shields.io/github/stars/radyalz/Dynomite?style=social)
![GitHub forks](https://img.shields.io/github/forks/radyalz/Dynomite?style=social)
![GitHub issues](https://img.shields.io/github/issues/radyalz/Dynomite)
![GitHub pull requests](https://img.shields.io/github/issues-pr/radyalz/Dynomite)
![GitHub last commit](https://img.shields.io/github/last-commit/radyalz/Dynomite)
![GitHub license](https://img.shields.io/github/license/radyalz/Dynomite)
![GitHub language top](https://img.shields.io/github/languages/top/radyalz/Dynomite)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/radyalz/Dynomite/ci.yml?label=CI&logo=github)

---

Welcome to an in-depth exploration of **Dynomite** — a high-performance, open-source **distributed in-memory key-value store** built by Netflix.

Dynomite extends the capabilities of Redis or Memcached by adding:

- **Cross-region replication**
- **Fault-tolerant clustering**
- **High availability**
- **Pluggable backends**
- **Eventually consistent storage**

Dynomite’s architecture is designed to provide Netflix-scale performance across global data centers.

---

## 🧠 What Dynomite Does

![Netflix Logo](images/NetflixLogo-resized.png)


Dynomite transforms single-node data stores (like Redis or Memcached) into a **peer-to-peer distributed system** by adding:

### ✔️ Peer-to-Peer Gossip-Based Communication

Dynomite uses gossip protocols to share node health and topology across the cluster.

### ✔️ Cross-DC Replication

You can replicate Redis data across different geographical regions with low-latency syncing.

### ✔️ Data Partitioning and Token Ring

Inspired by Cassandra, Dynomite uses virtual nodes and a consistent hash ring for partitioning and load balancing.

### ✔️ Pluggable Storage Engines

Currently supports:

- Redis (most commonly used)
- Memcached (experimental)

---

## 🖼 Architecture Overview

![Dynomite Architecture](images/dynomite-architecture.png)

> In this architecture, Dynomite nodes communicate across data centers using asynchronous replication. Each node wraps a Redis instance, handling replication and failover transparently.

---

## 🧾 Contents

- 📚 [Reading List](./MarkDowns/To-Read.md) — curated research papers, articles, and learning resources.
- 🗂️ [PDF Folders](./Pdfs) — notes and summaries from deep-dives into Dynomite and distributed systems.
- 🧠 [Dynomite Explained](./MarkDowns/ExplanationTSPProblem-no1.md) — detailed notes on how Dynomite works.
- 🧑‍🏫 [About Presentations](./MarkDowns/About-PowerPoint.md) — clean design tips for slides.
- 🐍 [Python Examples](./Code/Python/) — client test cases, Redis wrappers, and replication tests.
- 🛠️ [Deployment Examples](./Code/example.m) — coming soon (Docker/K8s deployments).

---

## 🔥 Dynomite in Production

Dynomite is used at **Netflix** to power highly-available, multi-region services with consistent, low-latency performance.

![Netflix Logo](images/netflix-logo.png)

Other companies exploring Dynomite include:

- [RocketFuel](https://rocketfuel.com)
- [Quotient](https://www.quotient.com/)
- [Various open-source adopters](https://github.com/Netflix/dynomite/network)

---

## 🛠 Suggestions / Contributions

Want to suggest a feature, tweak, or fix a typo? Open an issue or a pull request:

- 🔧 [Create an Issue](https://github.com/radyalz/Dynomite/issues)
- 🔄 [Make a Pull Request](https://github.com/radyalz/Dynomite/pulls)

> 🙌 All contributions — from configs and docs to new backends — are welcome!

---

## ⭐️ Favorite This Project

If you found this helpful, give it a ⭐️ — it helps more developers discover it!

---

## 🧪 Coming Soon

- 🧠 Cluster Simulations
- 🧰 Docker + Kubernetes Deployment Guides
- 🌐 Prometheus/Grafana Metrics Monitoring Setup
- 🧪 Stress-testing scripts

---

## 🗂 Folder Structure

```bash
📁 Dynomite/
├── 📁 Code/
│   └── Python/               # Python test scripts
├── 📁 MarkDowns/
│   ├── To-Read.md
│   ├── ExplanationTSPProblem-no1.md
│   └── About-PowerPoint.md
├── 📁 Pdfs/
├── 📁 images/                # Architecture diagrams, logos, etc.
│   ├── dynomite-architecture.png
│   └── netflix-logo.png
├── LICENSE
└── README.md
```
