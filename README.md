# Mayank Raj

**AI Software Engineer, Bengaluru.** I build production agentic systems — the agent runtime, the tool protocol, the retrieval layer, and the infrastructure they run on.

Most of my day job is in private repositories, so the graph below understates it. What I can share is here.

---

### Writing

**[Tool Calling Is a Distributed Systems Problem](https://github.com/mraj602/client-declared-tools)**
What happens to function calling once there is more than one caller, more than one service, and a client that knows things the server doesn't. Covers where tool configuration lives and when you resolve it, why filtering a tool list is not enforcement, the three architectures hiding under "client-declared tools", and how to budget timeouts down a serial chain so you stop telling users something failed after it succeeded.

More at **[medium.com/@mraj602](https://medium.com/@mraj602)**.

### Tools

**[typst-resume](https://github.com/mraj602/typst-resume)** — Write a résumé in Markdown, get a one-page ATS-parseable PDF. Pandoc → Typst, so it compiles in milliseconds and the template is readable by anyone who can read a scripting language.

---

### What I work on

**Agent runtimes and tool protocols.** Model Context Protocol, caller-scoped tool access, client-declared tool contracts over a realtime transport. Binding a model to a small set of discovery meta-tools so a growing catalog never inflates per-turn context cost.

**LLM platform engineering.** Provider-agnostic routing behind a gateway, tiering models by task difficulty with per-tier thinking budgets, and accounting for reasoning tokens separately — they are billed as output but are not part of the answer.

**Retrieval.** Embeddings and pgvector, grounding answers in a tenant's own data rather than model priors.

**Realtime voice.** LiveKit, streaming speech-to-text, and the particular problems of running voice on constrained embedded hardware.

**The layer underneath.** Kubernetes, Terraform, Helm and ArgoCD on AWS. I operate what I build — the gateway, the tracing plane and the media stack included.

**Guardrails for AI-assisted development.** Per-repository agent context, path-scoped rules, and a custom architecture-layering gate enforced on every pull request, so agent-generated code stays inside the architecture it was meant to respect.

---

`Python` · `FastAPI` · `Kotlin` · `LangGraph` · `LiteLLM` · `MCP` · `pgvector` · `LiveKit` · `Langfuse` · `Temporal` · `PostgreSQL` · `ClickHouse` · `Kubernetes` · `Terraform` · `AWS`
