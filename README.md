# Sideko (sideko)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Sideko is an API tooling generation platform that turns an OpenAPI specification into a complete developer-tooling suite — SDKs in six languages (Python, TypeScript, Java, Go, C#, Rust), Model Context Protocol (MCP) servers for AI agents, on-brand documentation sites with an Automatic MCP surface, mock servers, and CLI tooling — without writing generation code. The platform's "Hybrid Codegen" pairs deterministic OpenAPI-driven generation with guided AI customization, and ships LLM coding-assistant rule files (Claude Code, Cursor, Gemini, GitHub Copilot) alongside each SDK so agents can extend the generated code without breaking regeneration. Customers include Prudential Financial and Magic Hour AI; Sideko's published Stripe SDK benchmark generated over one million lines of SDK code in under sixty seconds.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- CLI
- Documentation
- Mock Servers
- Platform
- SDKs
- API Tooling
- SDK Generation
- MCP Generation
- AI
- Hybrid Codegen
- OpenAPI Linting

## Timestamps

- **Created:** 2025-01-30
- **Modified:** 2026-05-22

## APIs

### Sideko API

The Sideko REST API enables developers to programmatically manage API projects, generate SDKs in six languages (Python, TypeScript, Java, Go, C#, Rust), generate Model Context Protocol (MCP) servers from OpenAPI, lint specifications for generation-readiness, deploy mock servers, and publish on-brand API documentation sites. The API powers Sideko's "Hybrid Codegen" pipeline (deterministic generation plus guided AI customization) and ships LLM coding-assistant rules for Claude Code, Cursor, Gemini, and GitHub Copilot alongside each SDK.

- **Human URL:** [https://docs.sideko.dev/](https://docs.sideko.dev/)
- **Base URL:** `https://api.sideko.dev/v1`

#### Tags

- API Tooling
- SDK Generation
- MCP Generation
- Documentation
- Mock Servers
- OpenAPI Linting
- Platform

#### Properties

- [Documentation](https://docs.sideko.dev/)
- [OpenAPI](openapi/sideko-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/sideko-rules.yml)
- [Capabilities](capabilities/api-tooling-lifecycle.yaml)
- [JSON Schema](json-schema/sideko-api-project-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sideko-sdk-generation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/sideko-mcp-generation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/sideko-api-project-structure.json)
- [JSON-LD](json-ld/sideko-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/sideko-vocabulary.yml)
- [Plans](plans/sideko-plans-pricing.yml)
- [Rate Limits](rate-limits/sideko-rate-limits.yml)
- [Fin Ops](finops/sideko-finops.yml)
- [Example](examples/sideko-list-api-projects-example.json)
- [Example](examples/sideko-trigger-sdk-generation-example.json)
- [Example](examples/sideko-trigger-mcp-generation-example.json)
- [Example](examples/sideko-deploy-mock-server-example.json)
- [Sign Up](https://authentication.sideko.dev/sign-up)
- [Pricing](https://sideko.dev/pricing)
- [Git Hub](https://github.com/Sideko-Inc/sideko)

### Sideko CLI

The Sideko CLI is a Rust binary (current release v1.6.3, Aug 2025) that provides command-line access to the Sideko platform. Commands are organized into five resource groups — `sideko api` (create, version, lint, stats, download specs), `sideko sdk` (init, config, create, update, released for Python, TypeScript, Java, Go, C#, Rust, with optional GitHub Actions and LLM coding-assistant rule files for Claude Code, Cursor, Gemini, and GitHub Copilot), `sideko doc` (list, deploy), `sideko account`, and `sideko config`. Installs via Homebrew, pip, npm, or curl, and stores credentials in the OS-native secure store.

- **Human URL:** [https://github.com/Sideko-Inc/sideko](https://github.com/Sideko-Inc/sideko)

#### Tags

- CLI
- Developer Tools
- SDKs
- MCP
- OpenAPI Linting

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sideko)
- [Documentation](https://docs.sideko.dev/)
- [C L I Reference](https://github.com/Sideko-Inc/sideko/blob/main/docs/CLI.md)
- [Releases](https://github.com/Sideko-Inc/sideko/releases)
- [Install Script](https://github.com/Sideko-Inc/sideko/blob/main/install.sh)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko SDK Update Action

GitHub Action that keeps Sideko-generated SDKs up to date with their parent API. Runs `sideko sdk update` in CI, opens a versioned PR with the regenerated SDK, and preserves any custom files and LLM-coding-assistant rules. Repo is TypeScript, last updated March 2026.

- **Human URL:** [https://github.com/Sideko-Inc/sdk-update](https://github.com/Sideko-Inc/sdk-update)

#### Tags

- GitHub Action
- SDK Maintenance
- CI/CD

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sdk-update)
- [Git Hub Action](https://github.com/marketplace/actions/sideko-sdk-update)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko Node.js SDK

The Sideko Node.js SDK provides TypeScript and JavaScript bindings for the Sideko API. Generated by Sideko's own pipeline from the Sideko OpenAPI specification.

- **Human URL:** [https://github.com/Sideko-Inc/sideko-node-sdk](https://github.com/Sideko-Inc/sideko-node-sdk)

#### Tags

- SDK
- Node.js
- TypeScript
- JavaScript

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sideko-node-sdk)
- [SDK](https://www.npmjs.com/package/sideko-sdk)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko Python SDK

The Sideko Python SDK provides Python bindings for the Sideko API. Generated by Sideko's own pipeline from the Sideko OpenAPI specification.

- **Human URL:** [https://github.com/Sideko-Inc/sideko-python-sdk](https://github.com/Sideko-Inc/sideko-python-sdk)

#### Tags

- SDK
- Python

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sideko-python-sdk)
- [SDK](https://pypi.org/project/sideko-sdk/)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko Stripe TypeScript SDK (Sample)

Sample TypeScript SDK for the Stripe REST API, Sideko-generated as the benchmark behind the "Stripe API Challenge" blog post (over 1 million lines of SDK code generated in under 60 seconds). Demonstrates Sideko's scale and is the reference used in the Code Mode MCP benchmarks against raw MCP and CLI on 12 Stripe tasks.

- **Human URL:** [https://github.com/Sideko-Inc/sideko-stripe-typescript](https://github.com/Sideko-Inc/sideko-stripe-typescript)

#### Tags

- SDK
- Sample
- Stripe
- TypeScript

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sideko-stripe-typescript)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko Stripe Python SDK (Sample)

Sample Python SDK for the Stripe API, Sideko-generated as a companion to the TypeScript Stripe sample.

- **Human URL:** [https://github.com/Sideko-Inc/sideko-stripe-python](https://github.com/Sideko-Inc/sideko-stripe-python)

#### Tags

- SDK
- Sample
- Stripe
- Python

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sideko-stripe-python)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### make-request-py (Sideko Runtime)

Modern Python HTTP client library with built-in authentication and response handling, used as the runtime by Sideko-generated Python SDKs.

- **Human URL:** [https://github.com/Sideko-Inc/make-request-py](https://github.com/Sideko-Inc/make-request-py)

#### Tags

- HTTP Client
- Runtime
- Python

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/make-request-py)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### make-request-js (Sideko Runtime)

Modern TypeScript HTTP client for browser and Node.js environments, used as the runtime by Sideko-generated TypeScript SDKs.

- **Human URL:** [https://github.com/Sideko-Inc/make-request-js](https://github.com/Sideko-Inc/make-request-js)

#### Tags

- HTTP Client
- Runtime
- TypeScript
- JavaScript

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/make-request-js)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko SDK Reference

Boilerplate code used by Sideko to generate SDKs, including example SDKs that demonstrate the generated surface across supported languages.

- **Human URL:** [https://github.com/Sideko-Inc/sdk-reference](https://github.com/Sideko-Inc/sdk-reference)

#### Tags

- Boilerplate
- SDK
- Reference

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/sdk-reference)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sideko Homebrew Tap

Homebrew tap that publishes the `sideko` CLI binary (`brew install sideko-inc/tap/sideko`).

- **Human URL:** [https://github.com/Sideko-Inc/homebrew-tap](https://github.com/Sideko-Inc/homebrew-tap)

#### Tags

- Distribution
- Homebrew

#### Properties

- [Git Hub](https://github.com/Sideko-Inc/homebrew-tap)
- [Postman Collection](collections/sideko.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sideko.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/sideko)
- [Website](https://www.sideko.dev/)
- [Documentation](https://docs.sideko.dev/)
- [Sign Up](https://authentication.sideko.dev/sign-up)
- [Pricing](https://sideko.dev/pricing)
- [Blog](https://sideko.dev/resources)
- [Git Hub](https://github.com/Sideko-Inc)
- [Changelog](https://docs.sideko.dev/changelog/)
- [Terms of Service](https://www.sideko.dev/legal/terms)
- [Privacy Policy](https://www.sideko.dev/legal/privacy)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
