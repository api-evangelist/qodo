# Qodo (qodo)

Qodo (formerly CodiumAI) is an AI code-integrity platform for automated code review, test generation, and code quality across the SDLC. Its developer surface is delivered primarily as a hosted Git app and open-source PR-Agent (Qodo Merge), IDE plugins (Qodo Gen), and a terminal agent runtime (Qodo Command/CLI) rather than a broad public HTTP API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/qodo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/qodo/refs/heads/main/apis.yml)

## Tags

- AI
- Code Review
- Code Integrity
- Developer Tools
- Pull Requests

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Qodo Merge (PR-Agent)

AI pull-request reviewer. Available as the Apache-2.0 open-source PR-Agent (CLI, GitHub Action, Docker, self-hosted webhook server) and as the hosted Qodo Merge Git app. It is invoked through Git provider events and PR comment commands (/review, /describe, /improve, /ask) rather than a documented public REST API; self-hosted deployments expose a webhook HTTP endpoint that Git providers call.

- **Human URL:** [https://github.com/qodo-ai/pr-agent](https://github.com/qodo-ai/pr-agent)

#### Tags

- Code Review
- Pull Requests
- Git App
- Open Source

#### Properties

- [Documentation](https://docs.qodo.ai/code-review)
- [Source Code](https://github.com/qodo-ai/pr-agent)
- [OpenAPI](openapi/qodo-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/qodo.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/qodo.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Qodo Gen

AI pair-programmer delivered as JetBrains and VS Code IDE plugins for context-aware code generation, test generation, and documentation. It is an editor extension and does not expose a public HTTP API; integration is through the IDE marketplace plugins.

- **Human URL:** [https://www.qodo.ai/products/qodo-gen/](https://www.qodo.ai/products/qodo-gen/)

#### Tags

- IDE Plugin
- Test Generation
- Code Generation

#### Properties

- [Documentation](https://docs.qodo.ai)
- [JetBrains Plugin](https://plugins.jetbrains.com/plugin/21206-qodo-gen)
- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=Codium.codium)

### Qodo Command/CLI

Terminal runtime for building, running, and managing AI agents across the SDLC, installed via npm (@qodo/command). Agents can be exposed locally as HTTP services (--webhook), as a web UI (--ui), or as Model Context Protocol (MCP) servers (--mcp). These are user-hosted local services, not a documented hosted Qodo REST API.

- **Human URL:** [https://qodo.ai/products/qodo-gen-cli](https://qodo.ai/products/qodo-gen-cli)

#### Tags

- CLI
- Agents
- Automation
- MCP

#### Properties

- [Documentation](https://docs.qodo.ai)
- [Source Code](https://github.com/qodo-ai/command)
- [npm Package](https://www.npmjs.com/package/@qodo/command)

### Qodo Hosted API

The hosted Qodo platform that backs Qodo Merge, Qodo Gen, and Qodo Command. As of this writing Qodo does not publish a documented, general-purpose public HTTP REST API with stable endpoints; access is via the Git app, IDE plugins, and CLI. This entry is a placeholder for any future documented hosted API surface.

- **Human URL:** [https://docs.qodo.ai](https://docs.qodo.ai)

#### Tags

- Platform
- Hosted
- Integrations

#### Properties

- [Documentation](https://docs.qodo.ai)
- [OpenAPI](openapi/qodo-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/qodo-ai)
- [LinkedIn](https://www.linkedin.com/company/qodoai)
- [Website](https://www.qodo.ai)
- [Documentation](https://docs.qodo.ai)
- [Plans](plans/qodo-plans-pricing.yml)
- [Rate Limits](rate-limits/qodo-rate-limits.yml)
- [Fin Ops](finops/qodo-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
