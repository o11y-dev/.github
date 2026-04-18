```
                                  @@@@@@@@@@@
                                @@@@@@@@@@@@@@@
                               @@@@         @@@@
                              @@@@           @@@@
                            @@@@               @@@@
                           @@@@@               @@@@@
                          @@@@@@               @@@@@@
                        @@@@@@  (((((((((((((((  @@@@@@
                       @@@@  (((((((((((((((((((((  @@@@
                     @@@@  (((((((((((((((((((((((((  @@@@
                    @@@@ (((((((((           ((((((((( @@@@
                  @@@@@ ((((((((               (((((((( @@@@@
                 @@@@@@ ((((((((               (((((((( @@@@@@
               @@@@@@@  ((((((((               ((((((((  @@@@@@@
              @@@@      ((((((((               ((((((((      @@@@
             @@@@        (((((((((           (((((((((        @@@@
           @@@@            (((((((((((((((((((((((((            @@@@
          @@@@               (((((((((((((((((((((               @@@@
          @@@@                  (((((((((((((((                  @@@@
            @@@@         @@@@@@@@@@@@   @@@@@@@@@@@@         @@@@
             @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@

                    (((   (((                   @@
         @@@@@@@@ **.(( ** (( @@    @@    @@@@@@@@  @@@@@@@  @@    @@
         @@    @@    ((    (( @@    @@    @@    @@  @@@@@@@   @@@@@@
         @@@@@@@@    ((    (( @@@@@@@@ @@  @@@@@@@  @@@@@@@    @@@@
                               @@@@@@@
```

# o11y.dev — operational excellence for AI agents

Use telemetry and local session data to improve agent workflows. Produce observation scores, ship helper tools driven by telemetry, and give engineers a view into operational excellence for any AI coding agent.

Works with any AI coding agent that emits OTLP or writes a local session store. Currently supported: Antigravity, Claude Code, Cursor, Gemini CLI, GitHub Copilot, and OpenCode.

## Get started

```bash
pipx install o11y-reflect
reflect setup
reflect --demo
```

`reflect setup` wires all supported agents, starts a local OTLP gateway on `127.0.0.1:4317` / `:4318`, and installs skill packages for in-session analysis.

## Products

* **[reflect](https://reflect.o11y.dev/)** — hosted reports, observation scores, and skill/agent generation driven by telemetry. Reads OTLP and local session stores; runs in your terminal or browser.

* **[opentelemetry-hooks](https://github.com/o11y-dev/opentelemetry-hooks)** — the OpenTelemetry instrumentation layer that captures AI coding agent activity and emits OTLP. The data foundation underneath reflect.

* **[opentelemetry-skill](https://github.com/o11y-dev/opentelemetry-skill)** — observability knowledge for AI assistants. Helps configure native OpenTelemetry and interpret telemetry inline.

## Contribute

Explore the repos, open issues, or send PRs.

---

Built on OpenTelemetry GenAI semantic conventions. Vendor-neutral. Open source.
