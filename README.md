<p align="center">
  <img src="./profile_header.png" alt="header" width="100%" />
</p>

---

## ◈ About

Computer Science student focused on backend engineering, distributed systems, and cloud infrastructure. I enjoy building production-style systems, contributing to open source, and understanding how software behaves under load, failure, and scale.

---

## ◈ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,go,java&theme=dark&perline=8" alt="Languages" />
</p>
<p align="center"><sub><b>Languages</b></sub></p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=fastapi,postgres,redis,supabase&theme=dark&perline=8" alt="Backend & Databases" />
</p>
<p align="center"><sub><b>Backend & Databases</b></sub></p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=aws,docker,githubactions,linux&theme=dark&perline=8" alt="Cloud & DevOps" />
</p>
<p align="center"><sub><b>Cloud · DevOps · Tooling</b></sub></p>

<p align="center">
  <img src="https://skillicons.dev/icons?i=git,vscode&theme=dark&perline=8" alt="Tools" />
</p>
<p align="center"><sub><b>Tools & Workflow</b></sub></p>

---

## ◈ Featured Projects

<details>
<summary><b>⬡ CloudDrive — Production Cloud Storage Platform</b></summary>

<br>

A fully deployed cloud storage REST API serving real traffic at **clouddrive.world**, built with FastAPI and AWS. Designed for production-grade reliability with async processing, fine-grained access control, and multi-region availability.

<div align="center">

| Attribute | Detail |
|-----------|--------|
| **Stack** | Python · FastAPI · PostgreSQL · AWS S3 · AWS Lambda · Docker |
| **Auth** | IAM roles · presigned URLs · scoped access tokens |
| **Scale** | Multi-AZ deployment · active health checks · fault-tolerant routing |
| **Performance** | Async Lambda image processing · non-blocking upload/download pipelines |
| **Security** | IAM least-privilege · pre-signed URL expiry · parameterized queries |
| **Status** | Live at [clouddrive.world](https://clouddrive.world) |
| **Repository** | [github.com/Mauricio0129/CloudDrive](https://github.com/Mauricio0129/CloudDrive) |

</div>

Built the entire backend unilaterally — from schema design and auth architecture to AWS resource provisioning and CI/CD pipeline. Lambda functions handle asynchronous image processing without blocking the primary API request cycle. Multi-AZ health checks ensure uptime under node failure. Presigned S3 URLs offload bandwidth from the application tier while maintaining access control.

<br>
</details>

<details>
<summary><b>⬡ Layer 7 Load Balancer — High-Throughput Proxy in Go</b></summary>

<br>

A production-quality HTTP/1.1 reverse proxy written from scratch in Go, achieving **~79,000 requests/second** on commodity hardware. Built to demonstrate deep understanding of concurrent systems, network programming, and fault-tolerant architecture.

<div align="center">

| Attribute | Detail |
|-----------|--------|
| **Stack** | Go · net/http · sync/atomic · goroutines |
| **Performance** | ~79,000 req/sec sustained throughput |
| **Concurrency** | Lock-free atomic snapshots for backend pool state |
| **Reliability** | Two-tier health check system · automatic failover validated under load |
| **Security** | Adaptive read deadlines for slowloris attack mitigation |
| **Algorithm** | Round-robin with health-aware backend selection |
| **Repository** | [github.com/Mauricio0129/load-balancer](https://github.com/Mauricio0129/load-balancer) |

</div>

The core insight driving this implementation: lock-free atomic snapshots allow the hot path (request forwarding) to read backend state without ever acquiring a mutex, keeping latency consistent under high concurrency. The two-tier health check system separates liveness (fast, frequent) from readiness (deeper, less frequent) to avoid unnecessary failovers while still catching degraded backends. Adaptive read deadlines close connections that stall mid-request — a direct defense against slowloris-style attacks.

<br>
</details>

---

## ◈ Experience

**Independent Systems Engineering** · Personal Projects
`2024 – Present`

Designed, built, and deployed production systems independently — from architecture through CI/CD — across infrastructure, systems programming, and backend API development.

- Deployed CloudDrive, a live cloud storage API (clouddrive.world) with AWS Lambda, S3, and PostgreSQL
- Engineered a Layer 7 load balancer in Go achieving ~79k req/sec with lock-free concurrency
- Provisioned AWS IAM roles, multi-AZ configurations, and automated deployment pipelines

`Go` `Python` `AWS` `Docker` `FastAPI` `PostgreSQL` `GitHub Actions`

---


## ◈ Certifications

<p align="center">
  <b>AWS</b>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/AWS%20Developer%20Associate-In%20Progress-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS Dev Associate" />
  &nbsp;
  <img src="https://img.shields.io/badge/AWS%20Cloud%20Practitioner-Foundational-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS CCP" />
</p>

---


## ◈ Current Focus

```yaml
learning:
  - Profiling tools (pprof, py-spy) — understanding real performance vs. guessing
  - AWS Developer Associate certification

building:
  - Kafka-inspired message broker in Go

exploring:
  - Distributed consensus algorithms (Raft, Paxos)
  - Observability tooling (pprof, OpenTelemetry, Prometheus)
```

---

## ◈ Connect

<p align="center">
  <a href="https://www.linkedin.com/in/mauriciomoreno01/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
</p>

---

<p align="center">
  <sub><i>"Systems that survive production pressure aren't built by accident — they're built by engineers who understood the failure modes before writing a single line."</i></sub>
</p>
