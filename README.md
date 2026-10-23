# Mayank Raj

AI software engineer in Bengaluru. I build production agentic systems: agent runtimes, tool protocols (MCP), retrieval, and the infrastructure they run on. Recent work includes a LangGraph assistant serving tens of thousands of users over text and voice, and an agent pipeline cut from 7 model round-trips to 1 at 54% lower cost per task.

Most of my day-to-day work lives in private repositories. My open-source work is below.

---

## Switchyard

**[Switchyard](https://github.com/mraj602/switchyard)** is an open-source, self-hosted board for running many Claude Code accounts across many machines. It shows every session's state, every account's usage limits, and alerts you when a session needs you, all on a hub you run yourself.

- **One board** for every session on every machine, grouped by account: working, needs permission, asked a question, done, failed.
- **Usage limits** for every account (5-hour, 7-day, per model) with reset times and history.
- **Alerts** on a native Android app with its own connection to your hub (no Google push service, no proprietary Google code), or via Web Push, ntfy and desktop notifications.
- **Peers:** sessions in different accounts and on different machines can message each other, end-to-end encrypted; the hub relays ciphertext only.
- **Built as** a single static Go binary (`sy`) for the CLI and hub, plus a web board, an Electron desktop app and an Android app. AGPL-3.0.

[Repository](https://github.com/mraj602/switchyard) · [Website](https://mraj602.github.io/switchyard/) · [Releases](https://github.com/mraj602/switchyard/releases)

<sub>Switchyard is an unofficial, independent project. It is not affiliated with, endorsed by or sponsored by Anthropic. "Claude" and "Claude Code" are trademarks of Anthropic, PBC.</sub>

---

## What I work on

**Agent runtimes and tool protocols.** Model Context Protocol, caller-scoped tool access, and client-declared tool contracts over a realtime transport. Binding a model to a small set of discovery meta-tools, so a growing catalog never inflates per-turn context cost.

**LLM platform engineering.** Provider-agnostic routing behind a gateway, tiering models by task difficulty with per-tier thinking budgets, and accounting for reasoning tokens separately: they are billed as output but are not part of the answer.

**Retrieval.** Embeddings and pgvector, grounding answers in a tenant's own data rather than model priors.

**Realtime voice.** LiveKit, streaming speech-to-text, and running voice on constrained embedded hardware.

**The layer underneath.** Kubernetes, Terraform, Helm and ArgoCD on AWS. I operate what I build, including the gateway, the tracing plane and the media stack.

**Guardrails for AI-assisted development.** Per-repository agent context, path-scoped rules, and an architecture-layering gate on every pull request, so agent-generated code stays inside the architecture it was meant to respect.

---

## Writing

**[Tool Calling Is a Distributed Systems Problem](https://github.com/mraj602/client-declared-tools)**: what happens to LLM function calling once there is more than one caller, more than one service, and a client that knows things the server doesn't.

I write about building agent systems on **[Medium](https://medium.com/@mraj602)**.

## Stack

Python · Go · Kotlin · FastAPI · LangGraph · LiteLLM · MCP · pgvector · LiveKit · Langfuse · Temporal · PostgreSQL · ClickHouse · Kubernetes · Terraform · AWS

## Contact

GitHub [@mraj602](https://github.com/mraj602) · Medium [@mraj602](https://medium.com/@mraj602) · [mraj602@gmail.com](mailto:mraj602@gmail.com)
