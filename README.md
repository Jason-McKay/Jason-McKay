# Hi, I'm Jason 👋

Senior Java engineer. I build event-driven back ends with Spring Boot, Kafka and Redis, and I like documenting the decisions behind them.

## What I'm working on

### [Notification Platform](https://github.com/Jason-McKay/notification-platform)
An event-driven notification system: an HTTP ingress validates requests, dedupes them on an idempotency key in Redis and publishes to Kafka, and a separate worker consumes, dispatches and records delivery. Two deployables that scale and fail independently, with a shared contract module.
`Java 21` · `Spring Boot 4.1` · `Kafka` · `Redis` · `MySQL` · `Docker Compose`

### [Message Inspector](https://github.com/Jason-McKay/message-inspector) and [its UI](https://github.com/Jason-McKay/message-inspector-ui)
A browser tool for inspecting ActiveMQ Artemis JMS queues: browse messages, view pretty-printed JSON/XML payloads, and resend, delete or move messages to a dead-letter queue. JMS handles the message operations and Jolokia handles the queue discovery, a split explained in an ADR. It also ships an **MCP server**, so an AI agent such as Claude Code can list queues, browse messages and, with admin rights, move them to the DLQ. Every destructive call is role-checked and audit-logged.
`Java 21` · `Spring Boot 4.1` · `Artemis (JMS)` · `Redis` · `Angular 22` · `TypeScript` · `Spring AI / MCP`

## How I work
- **Decisions are written down.** Every non-obvious choice gets an architecture decision record (ADR) in the repo.
- **Security is part of the build.** CI runs OWASP dependency checks, and CVE overrides carry an expiry note.
- **Documented as I go.** Architecture diagrams and runnable examples in the READMEs.

## Coming next
- A delivery dashboard, retries and metrics for the Notification Platform

## Tools I use daily
`Java 21` · `Spring Boot` · `Kafka` · `Redis` · `Spring AI / MCP` · `Angular` · `Docker` · `MQL5` · `PowerShell`

## Contact
jasonm.mckay007@gmail.com
