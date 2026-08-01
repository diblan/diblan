# 👋 Hi, I'm Dieter (@diblan)

I'm a **senior software engineer** from Belgium, specialized in **Java/Spring backend systems** and platform modernization. In enterprise work at Volvo Cars, DXC Technology, and APB I migrated legacy stacks (Fortran/Java 6 → Java 17 / Spring Boot 3), replaced a legacy messaging system with **Kafka**, decomposed a government monolith into Spring Boot + Angular services behind Keycloak/OIDC, and moved deployments to **OpenShift** with IaC pipelines. Currently at Eniris, combining key-account work with hands-on engineering: Python, IoT integrations, and real-time monitoring on InfluxDB.

## 🤖 How I build now

My personal projects double as an ongoing experiment in **harness engineering**: designing the repo itself — agent guide, decision log, invariants, a verification script that only ever gets stricter — so that AI agents can do the implementation work reliably while I direct, review, and push. The current setup delegates across **two agents with asymmetric roles**: one as manager (specs, review, verification, commits), one as executor (implementation only, never commits). The code is agent-written; the judgment isn't.

## 🔭 Featured projects

- 💳 **[Payfold](https://github.com/diblan/payfold)** — a two-service Spring Boot billing stack: renewal producer/consumer over **RabbitMQ**, Postgres + Flyway, mock SEPA banks and PSP, DB-constraint idempotency (N parallel consumers can't double-bill), Testcontainers, Prometheus/Grafana, multi-arch images. Origin of the harness doctrine above.
- ☸️ **Homelab GitOps platform** *(private)* — the desired state of two Kubernetes clusters (k3d dev + single-node arm64 k3s) reconciled by **Flux**: SOPS-encrypted secrets, kube-prometheus-stack, and **KEDA** fanning payfold's consumer 1→5 on RabbitMQ queue depth — then collapsing it back after the drain. Built for depth over speed while relearning Kubernetes properly.
- 🧠 **[Othello neural-network trainer](https://github.com/diblan/othello)** — an AlphaZero-style self-play trainer in **Rust** ([Burn](https://burn.dev) + LibTorch on CUDA): MCTS-guided self-play, a CNN with policy/value heads, and arena gating where each new generation must beat the last.
- 📚 **[Qwizle](https://github.com/diblan/qwizle-codex)** — a daily learning & retention app (Spring Boot + Angular + Postgres), inspired by Wordle and Duolingo; a 2026 experiment in letting AI write all of the code while tracking where that breaks down.
- 🧪 **CV site A/B test** *(source private)* — one CV, two complete site implementations built independently by two different coding agents from the same brief, shipped in a single hardened nginx image that assigns each visitor an arm and keeps them on it.

## 🧰 Tech I enjoy

- **Java 17** — Spring Boot / Cloud / Data / Security, Hibernate, JUnit, Testcontainers
- **Messaging** — Kafka, RabbitMQ
- **Platform** — Docker, Kubernetes (Flux, KEDA, k3s), OpenShift, GitHub Actions, Azure DevOps
- **Data** — Postgres, Oracle, MongoDB, InfluxDB
- **Also** — Rust, Python, TypeScript/Angular

## 📜 Certificates

- **AWS Solutions Architect – Associate** (2025)
- **Oracle Certified Associate, Java SE 8** (2019)

📫 Reach me at: [dieter@blanchaert.com](mailto:dieter@blanchaert.com)
🔗 LeetCode: [leetcode.com/u/diblan](https://leetcode.com/u/diblan/)

---
"Code should outlive its creators."

<!---
diblan/diblan is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
