# Qodo (qodo)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
