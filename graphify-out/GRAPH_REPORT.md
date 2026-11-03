# Graph Report - .  (2026-11-03)

## Corpus Check
- 96 files · ~79,742 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 285 nodes · 346 edges · 20 communities (15 shown, 5 thin omitted)
- Extraction: 86% EXTRACTED · 14% INFERRED · 0% AMBIGUOUS · INFERRED: 48 edges (avg confidence: 0.84)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_API & MCP Access|API & MCP Access]]
- [[_COMMUNITY_Data Generation Steps|Data Generation Steps]]
- [[_COMMUNITY_Protocols & CI Integrations|Protocols & CI Integrations]]
- [[_COMMUNITY_Extensibility & Configuration|Extensibility & Configuration]]
- [[_COMMUNITY_RPC & HTTP Protocols|RPC & HTTP Protocols]]
- [[_COMMUNITY_Runs, Metrics & Automation|Runs, Metrics & Automation]]
- [[_COMMUNITY_Pro Protocol Drivers|Pro Protocol Drivers]]
- [[_COMMUNITY_CI and Protocol Guides RU|CI and Protocol Guides RU]]
- [[_COMMUNITY_Pro Features RU|Pro Features RU]]
- [[_COMMUNITY_Imports & Execution Lifecycle|Imports & Execution Lifecycle]]
- [[_COMMUNITY_Platform & Quick Start|Platform & Quick Start]]
- [[_COMMUNITY_Legal & Data Policies|Legal & Data Policies]]
- [[_COMMUNITY_Arrival-Rate Load Profiles|Arrival-Rate Load Profiles]]
- [[_COMMUNITY_PubSub Ack Modes|Pub/Sub Ack Modes]]
- [[_COMMUNITY_LLM & GPU Metrics|LLM & GPU Metrics]]
- [[_COMMUNITY_Typed Inputs|Typed Inputs]]
- [[_COMMUNITY_PubSub RU|Pub/Sub RU]]
- [[_COMMUNITY_FIX Message Tokens|FIX Message Tokens]]
- [[_COMMUNITY_Installation & Dev Stack|Installation & Dev Stack]]
- [[_COMMUNITY_AIO Documentation Sync|AIO Documentation Sync]]

## God Nodes (most connected - your core abstractions)
1. `Outbound webhook (per-workspace, HMAC-signed)` - 9 edges
2. `Библиотеки — WASM-генераторы токенов ${alias.fn(...)}` - 9 edges
3. `Libraries — WASM value-generator libraries for ${alias.fn(...)} tokens` - 8 edges
4. `Task run lifecycle (pending→running→passed|failed|cancelled|timeout)` - 8 edges
5. `Прогоны и живые метрики — жизненный цикл задачи` - 8 edges
6. `Test definition (statuses draft/active/archived)` - 7 edges
7. `Task (single execution of a test)` - 7 edges
8. `Cron trigger (schedule, machine, timezone, run now)` - 7 edges
9. `Database load testing from the CLI (PostgreSQL, MySQL/MariaDB, SQLite)` - 7 edges
10. `WebRTC pro module (full media path: ICE/DTLS-SRTP, RTP)` - 7 edges

## Surprising Connections (you probably didn't know these)
- `@std/json@v1 built-in library` --semantically_similar_to--> `std/read-json@v1 + общий JSON-кеш`  [INFERRED] [semantically similar]
  en/concepts/libraries.mdx → ru/concepts/files.mdx
- `std/thresholds@v1` --shares_data_with--> `Outbound webhook (per-workspace, HMAC-signed)`  [INFERRED]
  ru/getting-started/thresholds.mdx → en/concepts/webhooks.mdx
- `Условия использования (RU)` --semantically_similar_to--> `Terms of Service (EN)`  [INFERRED] [semantically similar]
  ru/terms.md → terms.md
- `Thresholds как SLO-пороги (std/thresholds@v1 в after:-блоке)` --semantically_similar_to--> `Thresholds as SLO gates (std/thresholds@v1 in the after: block)`  [INFERRED] [semantically similar]
  ru/getting-started/thresholds.mdx → en/getting-started/thresholds.mdx
- `abort_on_fail: true на пороге с severity: fail останавливает нагрузку досрочно` --semantically_similar_to--> `abort_on_fail: true on a severity: fail gate stops load early`  [INFERRED] [semantically similar]
  ru/getting-started/thresholds.mdx → en/getting-started/thresholds.mdx

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Three complementary JSON data-access mechanisms** — concepts_data_driven_steps_std_pick, concepts_files_jq_grammar, concepts_libraries_std_json [EXTRACTED 1.00]
- **Streaming during-run reporters family** — concepts_live_metrics_streaming_reporters, concepts_reports_builtin_reporters, concepts_live_metrics_backpressure [INFERRED 0.85]
- **WASM component extension points sharing the Library SDK** — concepts_custom_reporters_wit_contract, concepts_faker_wasm_library, concepts_libraries_capability_sandbox [INFERRED 0.75]
- **Four composable CI/CD integration paths (GitHub Action, GitLab CI, REST API, Webhooks)** — getting_started_ci_cd_github_action, getting_started_ci_cd_gitlab_ci, getting_started_ci_cd_rest_api, getting_started_ci_cd_webhooks [EXTRACTED 1.00]
- **Std-tier CLI protocol guides sharing the same YAML-to-metric-summary walkthrough shape** — getting_started_database_cli_database_testing, getting_started_graphql_cli_graphql_testing, getting_started_grpc_cli_grpc_testing, getting_started_websocket_cli_websocket_testing [INFERRED 0.85]
- **Paid Scale/Enterprise protocol capabilities rejected at creation time for Starter tenants** — pro_features_fix_fix_protocol, pro_features_soap_soap_protocol, pro_features_webrtc_webrtc_module, pro_features_pubsub_pubsub_drivers [EXTRACTED 1.00]
- **WASM-точки расширения движка: библиотеки, репортеры, faker** — concepts_libraries_doc, concepts_custom_reporters_doc, concepts_faker_doc, concepts_libraries_sandbox [INFERRED 0.85]
- **Наблюдаемость прогона: метрики, логи, отчёты, дашборд** — concepts_runs_doc, concepts_live_metrics_doc, concepts_protocol_metrics_doc, concepts_reports_doc [INFERRED 0.85]
- **Доступ к платформе: REST API, MCP, ASK AI** — api_reference_index_doc, api_reference_mcp_doc, concepts_ask_ai_doc [INFERRED 0.85]
- **Pro protocol features (FIX, SOAP, Pub/Sub, WebRTC) on Scale/Enterprise plans** — pro_features_fix_doc, pro_features_soap_doc, pro_features_pubsub_doc, pro_features_webrtc_doc [INFERRED 0.85]
- **Getting-started CLI protocol guides sharing the same install/run/lint/summary flow** — getting_started_database_cli_doc, getting_started_graphql_cli_doc, getting_started_grpc_cli_doc, getting_started_websocket_cli_doc, getting_started_webrtc_cli_doc [INFERRED 0.85]
- **CI/CD automation loop: pipelines trigger runs, thresholds gate, webhooks report back** — getting_started_ci_cd_doc, concepts_triggers_doc, concepts_webhooks_doc, getting_started_thresholds_doc [INFERRED 0.95]
- **abort_on_fail early-stop threshold gate** — en_getting_started_thresholds_abort_on_fail, en_getting_started_thresholds_monitor_250ms, en_getting_started_thresholds_after_summary_guaranteed, en_getting_started_thresholds_unknown_metric_warmup, ru_getting_started_thresholds_abort_on_fail [INFERRED 0.85]
- **http_debug masked failure-only diagnostics** — en_getting_started_thresholds_http_debug_error, en_getting_started_thresholds_abort_on_fail, ru_getting_started_thresholds_http_debug_error [INFERRED 0.85]

## Communities (20 total, 5 thin omitted)

### Community 0 - "API & MCP Access"
Cohesion: 0.06
Nodes (40): ApiError — общий формат ошибок (400/401/402/403/404/409/500/503), 402 PAYMENT_REQUIRED billing gate on /api/v1, Справочник API (REST API для BFF на Rust), API Reference — REST API for the perfscale BFF, Keycloak JWT bearer authentication (ROPC grant), Machine tokens (M2M client_credentials) for agents, openapi.json — машиночитаемый контракт OpenAPI, Personal API tokens (psk_…) with fine-grained scopes (+32 more)

### Community 1 - "Data Generation Steps"
Cohesion: 0.08
Nodes (35): Live metrics streaming & protocol-detecting Metrics dashboard, MCP run tools (run_test, list_runs, get_run, get_run_logs, runs_by_machine), Run history with plan-based retention (30/90/365 days), Task run lifecycle (pending→running→passed|failed|cancelled|timeout), Tasks REST API (POST/DELETE /api/v1/tasks), Тесты и задачи, Result metrics (p50/p95/p99/errorRate/requestsPerSec/totalRequests), Supported load tools (k6, JMeter, Locust, Artillery, Gatling, custom) (+27 more)

### Community 2 - "Protocols & CI Integrations"
Cohesion: 0.07
Nodes (34): Conditional steps if:/when: (equivalent aliases), Data-driven шаги (if/when, std/random, std/pick, per-VU переменные), Data-driven steps — conditions, std/random, std/pick, per-VU variables, std/pick@v1 — выбор элемента JSON-массива, std/random@v1 — шаг генерации числа, std/pick@v1 step — dynamic array selection, std/random@v1 step, Per-VU variables ${{ __vu__ }} / ${{ __iter__ }} (+26 more)

### Community 3 - "Extensibility & Configuration"
Cohesion: 0.08
Nodes (29): Message assertions via std/check@v1 (any quantifier, by-index addressing), Live WS connection (std/ws-connect/send/recv/ping/close@v1), ws_msg_rtt application-level message RTT metric, std/ws@v1 one-shot WebSocket session, Data retention (30-day purge after deletion; 7-year financial records), perfscale Privacy Policy (effective 2026-04-03), Stripe (payment processor; raw card numbers not stored), User data rights (access, correction, deletion, portability, objection; GDPR/EU servers) (+21 more)

### Community 4 - "RPC & HTTP Protocols"
Cohesion: 0.10
Nodes (26): Perfscale/allure2-reporter — production-пример WASM-репортера, Контракт perfscale:reporter@0.1.0 (WIT, emit-file, report@v1), Свой репортер — WASM-компонент perfscale:reporter@0.1.0, Custom reporters — WASM reporter components, Perfscale/github-action, @perfscale/library-sdk TypeScript SDK, Reporter sandbox — emit-file is the only output channel, perfscale:reporter@0.1.0 WIT contract (+18 more)

### Community 5 - "Runs, Metrics & Automation"
Cohesion: 0.10
Nodes (25): std/graphql@v1 (интроспекция, schema_file, метрики graphql_*), GraphQL — std/graphql@v1 с валидацией по схеме, GraphQL load testing — std/graphql@v1, GraphQL failure semantics (errors in 200 OK body), Schema-aware validation via introspection or schema_file, Шаги std/grpc*@v1 (grpc, grpc-connect, grpc-call, grpc-stream-*), gRPC — unary и client/server/bidi-стримы, динамические схемы, gRPC load testing — std/grpc* steps (+17 more)

### Community 6 - "Pro Protocol Drivers"
Cohesion: 0.10
Nodes (21): webrtc_* CLI metric summary (setup_ms, ttff_ms, rtt, bitrate, call errors), WebRTC load testing from the CLI (WHIP publish, P2P calls), FIX protocol load testing (paid, Scale/Enterprise), Kafka driver via rdkafka (manual partition assignment, SASL), MQTT driver (v3.1.1, QoS 0-2, rustls TLS), Pro pub/sub drivers for std/pubsub@v1 (Redis, MQTT, Kafka), Redis Pub/Sub driver (fire-and-forget, subscribe-first), One Redis atomic command per op (INCRBY/RPUSH/LPOP/SET/GET) (+13 more)

### Community 7 - "CI and Protocol Guides RU"
Cohesion: 0.16
Nodes (15): abort_on_fail: true on a severity: fail gate stops load early, after: teardown, reporters, and the final summary still run after an abort, http_debug: error — one secret-masked JSON line per failed action/check with request/response payloads; success emits nothing, Gate evaluated every 250 ms during the VU phase; stops between steps, run.threshold_failed webhook event on the platform, Thresholds as SLO gates (std/thresholds@v1 in the after: block), std/thresholds@v1 action, A gate whose metric has no samples yet waits for data instead of aborting (+7 more)

### Community 8 - "Pro Features RU"
Cohesion: 0.18
Nodes (15): WebRTC из CLI, pro/fix* actions, CoinAPI Market Data FIX venue (fix.coinapi.io:3303), FIX data dictionary loaded from venue spec (QuickFIX FIX44.xml), Протокол FIX, pro/fix@v1 session action (logon, messages, logout, timed), pro/fix-config@v1 reusable connection profile, Pub/Sub — Redis, MQTT, Kafka (+7 more)

### Community 9 - "Imports & Execution Lifecycle"
Cohesion: 0.25
Nodes (11): std/ws* action family, WebSocket, std/db-* action family, Базы данных из CLI, std/graphql@v1, GraphQL из CLI, std/grpc-* action family, gRPC из CLI (+3 more)

### Community 10 - "Platform & Quick Start"
Cohesion: 0.22
Nodes (10): Импорт документов (import:, deep-merge, fail-closed сеть), --allow-remote-import и изоляция источников (URL/git), Arrival-rate — открытая модель, dropped_iterations, queue wait метрики, Профили нагрузки (fixed, stages, arrival-rate), allow_process_actions safety gate, before:/after: setup & teardown blocks, std/child_process@v1 (spawn sidecar process with readiness gate and restart policy), Setup и teardown (before:/after:, child_process, kill_process) (+2 more)

### Community 11 - "Legal & Data Policies"
Cohesion: 0.70
Nodes (5): Terms of Service (EN), Политика конфиденциальности (RU), Infrastructure providers (AWS, Hetzner), Stripe (payment processor), Условия использования (RU)

### Community 12 - "Arrival-Rate Load Profiles"
Cohesion: 0.67
Nodes (3): Arrival-rate open model with dropped_iterations, Load profiles — fixed, stages, arrival-rate, Open-model latency metrics (engine_arrival_queue_wait_ms, engine_arrival_iteration_ms)

### Community 13 - "Pub/Sub Ack Modes"
Cohesion: 0.67
Nodes (3): Pub/Sub load testing — std/pubsub@v1, Pub/Sub drivers (memory, nats; pro: kafka/redis/mqtt), Connection posture (scope) and publish ack mode (flush)

### Community 14 - "LLM & GPU Metrics"
Cohesion: 0.67
Nodes (3): LLM и GPU метрики, nvidia-smi-pro GPU collector, pro_llm_* metrics (ITL/TPOT percentiles, cost)

## Ambiguous Edges - Review These
- `perfscale SaaS load testing platform` → `perfscale Privacy Policy (effective 2026-04-03)`  [AMBIGUOUS]
  privacy.md · relation: conceptually_related_to

## Knowledge Gaps
- **112 isolated node(s):** `Update AIO GitHub Actions workflow`, `Perfscale/aio repository (docs gitlink bump target)`, `site repo git submodule inclusion (content/)`, `Fine-grained token scopes (tests/runs/machines/metrics read-write)`, `Generative UI — fixed component vocabulary with run actions` (+107 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **5 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `perfscale SaaS load testing platform` and `perfscale Privacy Policy (effective 2026-04-03)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Perfscale/github-action (run-and-gate workflow step)` connect `Extensibility & Configuration` to `Data Generation Steps`?**
  _High betweenness centrality (0.072) - this node is a cross-community bridge._
- **Why does `Интеграция с CI/CD` connect `Data Generation Steps` to `Imports & Execution Lifecycle`, `Extensibility & Configuration`?**
  _High betweenness centrality (0.066) - this node is a cross-community bridge._
- **Why does `Прогоны и живые метрики — жизненный цикл задачи` connect `Runs, Metrics & Automation` to `API & MCP Access`, `RPC & HTTP Protocols`?**
  _High betweenness centrality (0.060) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Outbound webhook (per-workspace, HMAC-signed)` (e.g. with `Task (single execution of a test)` and `std/thresholds@v1`) actually correct?**
  _`Outbound webhook (per-workspace, HMAC-signed)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Update AIO GitHub Actions workflow`, `Perfscale/aio repository (docs gitlink bump target)`, `site repo git submodule inclusion (content/)` to the rest of the system?**
  _113 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `API & MCP Access` be split into smaller, more focused modules?**
  _Cohesion score 0.06025641025641026 - nodes in this community are weakly interconnected._