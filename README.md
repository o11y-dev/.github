# .github

Shared org standards and public-facing entry points for **o11y.dev**.

Core product direction:

- **`reflect`** is the main entry point for setup, analysis, and reporting
- **`reflect gateway`** is the default local OTLP intake layer on port `4317` (OTLP gRPC) and port `4318` (OTLP HTTP)
- **`~/.reflect/state/`** is the default local storage location for traces, logs, and sessions
- **`reflect gateway`** is also the current path for team/shared forwarding into Coralogix
- **`opentelemetry-hooks`** is the capture/control layer when hook-based instrumentation is needed
- **`opentelemetry-skill`** is the setup and observability guide

Positioning guidance:

- aim at engineering leaders and platform teams, not only individual developers
- emphasize local-first control, clear deployment paths, and compatibility with existing observability stacks
- do not overclaim enterprise readiness; frame the product as practical today and expanding toward enterprise rollout patterns
