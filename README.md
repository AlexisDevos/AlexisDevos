# Alexis Devos

**Product engineer building AI agents that hold up in production** — connected to real tools and real data, measured by evals, watched by monitoring, and kept in check by human approval.

Founder & CTO of [Astrée](https://astree.online), a document-intelligence product for law firms, in production. Based in Paris. **Open to a full-time role building and operating AI agents** (Paris or remote), as well as focused missions.

## What I do

- Build agents and the connectors they need: mailboxes, cloud drives, calendars, legal databases, MCP servers.
- Make them reliable: idempotent background jobs, prompt regression evals, prompt-injection defenses, approval gates, deterministic tests.
- Monitor them: error tracking, Prometheus metrics, centralized logs, LLM cost and budget tracking.
- Ship the whole product around them with TypeScript, Python, Rust, PostgreSQL and Redis, and talk with the people who use it.

## AI agents

| Project | What it demonstrates |
| --- | --- |
| [Astrée](https://github.com/AlexisDevos/astree-case-study), in production | Gmail triage, Google Drive import (OAuth and push webhooks), deadline extraction to calendar, legal watch and a morning briefing, run as about twenty BullMQ job types. 10 promptfoo regression suites, including prompt injection through documents and RAG citation grounding. Sentry with PII scrubbing, a Prometheus endpoint, and logs and Redis/BullMQ metrics shipped to Grafana through Alloy |
| [Astrée Agent](https://github.com/AlexisDevos/astree-agent-case-study), prototype | An always-on legal agent in Rust, about 110,000 lines and nearly 800 tests: the model proposes, a gateway decides. Approvals are bound to the exact action, single-use and expire after 15 minutes; an incoming email is data, never an order. Proof tests with trapped emails, evals on a synthetic law firm, 15 ADRs |

## Other selected work

| Project | What it demonstrates |
| --- | --- |
| [dsh-remote-vps](https://github.com/AlexisDevos/dsh-remote-vps) | Rust agent, SSH confinement, gRPC, systemd hardening and atomic file operations |
| [Grok Bot — VPS sandbox & test suite](https://github.com/AlexisDevos/grok-bot-0.18-reconstructed) | Electron/host boundaries, remote sandbox connector, credential lifecycle, 69/69 deterministic tests on a reconstruction by [@b-nnett](https://github.com/b-nnett) |

## Open-source engineering

Work on other people's runtimes, where the bar is someone else's review:

- **[T3 Code #7331](https://github.com/pingdotgg/t3code/issues/7331)** — DeepSeek Harness provider integration: driver, adapter, JSON-RPC runtime, streaming, model discovery and headless generation.
- **[DeepSeek Harness #2888](https://github.com/deepseek-ai/deepseek-harness/discussions/2888)** — SDK wire lifecycle: `session/cancel` and `session/close`, 107/107 tests, lint and typecheck green.
- **[Command Code #371](https://github.com/CommandCodeAI/command-code/issues/371)** — Diagnosed an MCP process leak: orphaned Python processes accumulating across sessions to 60 processes and 1.52 GB, traced to `detached: true` + `.unref()`.

## Technical focus

`TypeScript` · `Python` · `Rust` · `Next.js` · `FastAPI` · `PostgreSQL` · `Redis/BullMQ` · `AI SDKs` · `MCP` · `promptfoo` · `Sentry` · `Grafana` · `Docker` · `CI/CD` · `security`

## Contact

- Website: [astree.online](https://astree.online)
- LinkedIn: [alexis4astree](https://www.linkedin.com/in/alexis4astree/)

For a full-time role on AI agents, a product build or an architecture review, [send me a message](https://www.linkedin.com/in/alexis4astree/).
