<div align="center">

<img alt="Pepe drinking coffee and coding" width="260" src="./assets/pepe-animated.gif" />

### Akshat Anand

SDE2 @ Barclays · backend, distributed systems, AI agents, Inference

**22 PRs merged upstream** into vLLM, vLLM-Omni, SGLang, NVIDIA Dynamo, Kubernetes and VS Code

[LinkedIn](https://www.linkedin.com/in/akshatanand1999) · [Twitter](https://twitter.com/hey_akshat) · [Email](mailto:akshatanandmallik@gmail.com)

</div>

---

**About me**

Akshat Anand is a Software Development Engineer II (SDE2) at Barclays, based in India, working on backend systems, distributed systems, LLM inference and AI agents. He has 22 pull requests merged into open-source projects including vLLM, SGLang, NVIDIA Dynamo, Kubernetes and VS Code.

```yaml
name: Akshat Anand
title: Software Development Engineer II (SDE2)
company: Barclays
location: India
roles:
  - Backend Engineer
  - Distributed Systems Engineer
  - LLM Inference Engineer
  - AI Agents Engineer
certifications:
  - AWS Certified Cloud Practitioner: https://www.credly.com/badges/d2a21830-7ca1-465c-bd95-3eb4e5187224/public_url
  - AWS Certified AI Practitioner: https://www.credly.com/badges/b7864762-eaf0-4cd8-8079-d89291e7159c/public_url
skills:
  languages: [Java, Go, Python, TypeScript]
  backend: [Spring Boot, FastAPI, REST APIs, gRPC, Microservices]
  data: [Apache Kafka, PostgreSQL, Redis, pgvector]
  distributed_systems:
    - Event-driven architecture
    - Transactional outbox
    - Idempotency
    - Prometheus observability
  llm_inference: [vLLM, SGLang, NVIDIA Dynamo, KV cache, Sampling kernels]
  ai_agents: [RAG, LangGraph, Tool calling, Multi-agent systems]
  cloud_devops: [AWS, Docker, Kubernetes, GitHub Actions, Cloudflare Workers]
open_source:
  merged_prs: 22
  projects:
    - vLLM
    - vLLM-Omni
    - SGLang
    - NVIDIA Dynamo
    - Kubernetes
    - VS Code
    - Playwright
    - Appwrite
    - Apple Pkl
```

**Recent contributions · 2026**

- ✅ **vLLM**: stop the Olmo3 tool parser dropping streamed text that starts with `<` ([#65936](https://github.com/vllm-project/vllm/pull/65936))
- ✅ **vLLM**: warn at startup when secondary-tier offloaded KV is tied to the parallel config ([#62566](https://github.com/vllm-project/vllm/pull/62566))
- ✅ **NVIDIA Dynamo**: keep multimodal routing opt-in so default wheel builds stop compiling the image stack ([#18199](https://github.com/ai-dynamo/dynamo/pull/18199))
- ✅ **NVIDIA Dynamo**: wait for the KAI queue controller before creating Dynamo queues in the Helm chart ([#16723](https://github.com/ai-dynamo/dynamo/pull/16723))
- ✅ **VS Code**: release `code -w -g file:line` once the file's editor closes ([#344740](https://github.com/microsoft/vscode/pull/344740))
- ✅ **NVIDIA Dynamo**: end-to-end AICR installation guide for Kubernetes ([#16416](https://github.com/ai-dynamo/dynamo/pull/16416))
- ✅ **vLLM-Omni**: place stage-CLI test replicas on separate GPUs ([#9041](https://github.com/vllm-project/vllm-omni/pull/9041))
- ✅ **VS Code**: keep the paused debug location range valid in chat ([#342379](https://github.com/microsoft/vscode/pull/342379))
- ✅ **vLLM**: serve Gemma 4 on `/v1/systemone` and `/v1/decisions` ([#62303](https://github.com/vllm-project/vllm/pull/62303))
- ✅ **SGLang**: clamp glm4v request video budgets to the deployment limit ([#43871](https://github.com/sgl-project/sglang/pull/43871))
- ✅ **vLLM**: carry the boundary tie count across blocks in the split top-p mask kernel ([#62046](https://github.com/vllm-project/vllm/pull/62046))
- ✅ **vLLM**: reject mismatched float16/bfloat16 KV cache dtype ([#60885](https://github.com/vllm-project/vllm/pull/60885))
- ✅ **NVIDIA Dynamo**: keep NIXL telemetry capture when export is disabled ([#15570](https://github.com/ai-dynamo/dynamo/pull/15570))
- ✅ **SGLang**: skip diffusion warmup preload when it would OOM ([#40761](https://github.com/sgl-project/sglang/pull/40761))
- ✅ **Kubernetes**: `_total` suffix for the endpoint slice controller metric ([#140447](https://github.com/kubernetes/kubernetes/pull/140447))
- ✅ **VS Code**: center Modern UI panel title tabs in the 32px header ([#331612](https://github.com/microsoft/vscode/pull/331612))
- ✅ **VS Code**: Modern UI tabs reserve the close-button column so it doesn't overlay the filename ([#330754](https://github.com/microsoft/vscode/pull/330754))
- ✅ **Appwrite**: return ISO8601 session expire from `updateSession` ([#12891](https://github.com/appwrite/appwrite/pull/12891))
- ✅ **Playwright**: pass client name on token-bypass connect ([#41845](https://github.com/microsoft/playwright/pull/41845))
- ✅ **VS Code**: fix Modern UI editor tab decoration color on full label ([#325291](https://github.com/microsoft/vscode/pull/325291))
- ✅ **Apple Pkl**: fix super method call inside a `let` expression ([#1383](https://github.com/apple/pkl/pull/1383))

<sub>✅ merged upstream · newest first</sub>

<details>
<summary>2025</summary>

- ✅ **DigitalOcean Gradient**: `wait_until_ready()` for agent deployments ([#56](https://github.com/digitalocean/gradient-python/pull/56))

</details>

**Projects**

- **[antibody](https://github.com/cipheraxat/antibody)**: every fix becomes a Semgrep rule your AI coding agent can't break, enforced on agent edits and in CI.<br>Python · Semgrep · static analysis · Claude Code
- [nanoserve](https://github.com/cipheraxat/nanoserve): small vLLM-style inference engine with paged KV cache, continuous batching and prefix caching.<br>Python · PyTorch · Triton · OpenAI-compatible server
- [codereviewer_agent](https://github.com/cipheraxat/codereviewer_agent): multi-agent GitHub Action that posts only fact-checked, high-confidence inline PR comments.<br>Python · LangGraph · RAG · pgvector · GitHub Actions
- [a2a-incident-agents](https://github.com/cipheraxat/a2a-incident-agents): incident diagnosis and remediation agents with approval gates, traces and evals.<br>Java 21 · Spring Boot · Spring AI · Postgres + pgvector
- [usage-billing-pipeline](https://github.com/cipheraxat/usage-billing-pipeline): exactly-once usage billing with Redis dedup, a transactional outbox and a DLQ.<br>Go · Kafka · Redis · PostgreSQL · Prometheus
- [CopilotPulse](https://github.com/cipheraxat/CopilotPulse): local-first VS Code extension with dashboards for Copilot Chat sessions, tokens and per-model cost.<br>TypeScript · React · VS Code API
- [briefly](https://github.com/cipheraxat/briefly): AI briefing agent whose durable workflow plans, drafts, revises and saves briefs, with persistent memory.<br>TypeScript · Cloudflare Workers AI · Durable Objects · Workflows

---

<sub>Marathons · weight training · too many terminal tabs</sub>
