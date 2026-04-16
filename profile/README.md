![o11y.dev observability engineering banner](https://raw.githubusercontent.com/o11y-dev/.github/main/profile/o11y-dev-observability-engineering-banner.jpeg)

# o11y.dev 🔭

**Observability for AI engineering workflows**

o11y.dev helps teams see **where tokens, retries, tool failures, and latency actually go** across tools like Claude Code, GitHub Copilot, Gemini CLI, Codex, and Cursor.

Instead of guessing why an agent hit limits, got stuck in a loop, or quietly burned budget, you can capture telemetry locally, inspect it with `reflect`, and route it through infrastructure you control.

## ⚡ Fastest way to try it

```bash
pipx install o11y-reflect
reflect setup
reflect --demo
```

`reflect setup` wires supported agents, starts a local OTLP gateway on `127.0.0.1:4317` / `:4318`, and writes telemetry to `~/.reflect/state/`.

## 🏢 Built for teams, usable today

- **Local-first by default** for fast evaluation and developer trust
- **Shared gateway path** when teams want centralized forwarding and observability
- **No forced SaaS control plane** to get value from the product
- **Current maturity, clear direction**: practical now for engineering teams, expanding toward enterprise rollout patterns

## ✨ Recent developments

- **Local OTLP gateway** with `reflect gateway {start|stop|status}`
- **Health and drift checks** with `reflect doctor` and `reflect update`
- **Reusable skill extraction** from session history with `reflect skills`
- **Hosted and local dashboards** from the same local-first telemetry pipeline

## 🚀 Featured Projects

* 🔭 **[reflect](https://github.com/o11y-dev/reflect)**  
  *The main entry point.* Install telemetry, run `reflect gateway`, compare agents, inspect token/tool behavior, and render terminal, markdown, or hosted dashboard views.

* 🪝 **[opentelemetry-hooks](https://github.com/o11y-dev/opentelemetry-hooks)**  
  *The capture layer when you need control.* Add hook-based spans, logs, and process-boundary observability for AI tools.

* 🧠 **[opentelemetry-skill](https://github.com/o11y-dev/opentelemetry-skill)**  
  *The observability guide.* Helps configure native OpenTelemetry first and use hooks only when you need more control.

## 🎯 What you should understand in seconds

- this is for engineering teams adopting AI coding tools
- this helps explain limits, retries, loops, spend, and tool failure patterns
- `reflect` is the easiest place to start
- nothing needs a cloud account to get value locally
- the architecture can grow from individual use to team-level telemetry

## 📊 What you get

- local-first telemetry capture and analysis
- terminal dashboard, markdown report, and browser dashboard output
- side-by-side agent comparison across supported tools
- actionable recommendations from your own workflow data

## 🧭 Deployment shape

- **Developer workstation**: `reflect` + local gateway + local state
- **Team/shared path**: OTLP into `reflect gateway` for forwarding into Coralogix
- **Instrumentation choice**: native OpenTelemetry first, hooks when deeper control is needed

## 🧭 Product shape

- **`reflect`** = setup, analysis, and reporting
- **`reflect gateway`** = local OTLP intake on `4317/4318`
- **`~/.reflect/state/`** = default local trace, log, and session storage
- **`opentelemetry-hooks`** = control-loop and capture layer
- **`opentelemetry-skill`** = setup guidance

## 🤝 Contribute

We are actively building the local-first path for understanding AI workflow behavior. Explore the repos, test the setup, open issues, or send PRs.
  
---
*Visit our [repositories](https://github.com/orgs/o11y-dev/repositories) to see what we're working on today.*
