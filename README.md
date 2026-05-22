# Sideko (sideko)

Sideko is an API tooling generation platform that turns an OpenAPI specification into a complete developer-tooling suite — SDKs in six languages (Python, TypeScript, Java, Go, C#, Rust), Model Context Protocol (MCP) servers for AI agents, on-brand documentation sites with an Automatic MCP surface, mock servers, and CLI tooling — without writing generation code. The platform's "Hybrid Codegen" pairs deterministic OpenAPI-driven generation with guided AI customization, and ships LLM coding-assistant rule files (Claude Code, Cursor, Gemini, GitHub Copilot) alongside each SDK so agents can extend the generated code without breaking regeneration. Customers include Prudential Financial and Magic Hour AI; Sideko's published Stripe SDK benchmark generated over one million lines of SDK code in under sixty seconds.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

CLI, Documentation, Mock Servers, Platform, SDKs, API Tooling, SDK Generation, MCP Generation, AI, Hybrid Codegen, OpenAPI Linting

## Timestamps

- **Created:** 2025-01-30
- **Modified:** 2026-05-22

## APIs

### Sideko API

The Sideko REST API enables developers to programmatically manage API projects, generate SDKs in six languages (Python, TypeScript, Java, Go, C#, Rust), generate Model Context Protocol (MCP) servers from OpenAPI, lint specifications for generation-readiness, deploy mock servers, and publish on-brand API documentation sites.

**Human URL:** [https://docs.sideko.dev/](https://docs.sideko.dev/)

**Base URL:** https://api.sideko.dev/v1

**Tags:** API Tooling, SDK Generation, MCP Generation, Documentation, Mock Servers, OpenAPI Linting, Platform

#### Properties

- [Documentation](https://docs.sideko.dev/)
- [OpenAPI](openapi/sideko-openapi.yml)
- [Spectral Rules](rules/sideko-rules.yml)
- [Capabilities (workflow)](capabilities/api-tooling-lifecycle.yaml)
- [JSON Schema — API Project](json-schema/sideko-api-project-schema.json)
- [JSON Schema — SDK Generation](json-schema/sideko-sdk-generation-schema.json)
- [JSON Schema — MCP Generation](json-schema/sideko-mcp-generation-schema.json)
- [JSON Structure — API Project](json-structure/sideko-api-project-structure.json)
- [JSON-LD Context](json-ld/sideko-context.jsonld)
- [Vocabulary](vocabulary/sideko-vocabulary.yml)
- [Plans & Pricing](plans/sideko-plans-pricing.yml)
- [Rate Limits](rate-limits/sideko-rate-limits.yml)
- [FinOps](finops/sideko-finops.yml)

### Sideko CLI

The Sideko CLI is a Rust binary (current release v1.6.3, Aug 2025) with five resource groups — `sideko api`, `sideko sdk`, `sideko doc`, `sideko account`, `sideko config` — including SDK generation for Python, TypeScript, Java, Go, C#, and Rust with optional GitHub Actions and LLM coding-assistant rules (Claude Code, Cursor, Gemini, GitHub Copilot). Installs via Homebrew, pip, npm, or curl.

**Human URL:** [https://github.com/Sideko-Inc/sideko](https://github.com/Sideko-Inc/sideko)

**Tags:** CLI, Developer Tools, SDKs, MCP, OpenAPI Linting

### Sideko SDK Update Action

GitHub Action that keeps Sideko-generated SDKs in sync with their parent API by running `sideko sdk update` in CI and opening a versioned PR with the regenerated code.

**Human URL:** [https://github.com/Sideko-Inc/sdk-update](https://github.com/Sideko-Inc/sdk-update)

### Sideko Node.js SDK

The Sideko Node.js SDK provides TypeScript and JavaScript bindings for the Sideko API.

**Human URL:** [https://github.com/Sideko-Inc/sideko-node-sdk](https://github.com/Sideko-Inc/sideko-node-sdk)

### Sideko Python SDK

The Sideko Python SDK provides Python bindings for the Sideko API.

**Human URL:** [https://github.com/Sideko-Inc/sideko-python-sdk](https://github.com/Sideko-Inc/sideko-python-sdk)

### Sideko Stripe TypeScript SDK (Sample)

Sample TypeScript SDK for the Stripe REST API, Sideko-generated as the benchmark behind the "Stripe API Challenge" blog post (over 1 million lines of SDK code generated in under 60 seconds) and the reference used in Code Mode MCP benchmarks.

**Human URL:** [https://github.com/Sideko-Inc/sideko-stripe-typescript](https://github.com/Sideko-Inc/sideko-stripe-typescript)

### Sideko Stripe Python SDK (Sample)

Sample Python SDK for the Stripe API, Sideko-generated as a companion to the TypeScript Stripe sample.

**Human URL:** [https://github.com/Sideko-Inc/sideko-stripe-python](https://github.com/Sideko-Inc/sideko-stripe-python)

### make-request-py & make-request-js (Sideko Runtimes)

The HTTP-client runtimes used by Sideko-generated SDKs.

- [make-request-py](https://github.com/Sideko-Inc/make-request-py)
- [make-request-js](https://github.com/Sideko-Inc/make-request-js)

### Sideko SDK Reference

Boilerplate code and example SDKs that Sideko uses to generate target-language SDKs.

**Human URL:** [https://github.com/Sideko-Inc/sdk-reference](https://github.com/Sideko-Inc/sdk-reference)

### Sideko Homebrew Tap

Homebrew tap publishing the `sideko` CLI (`brew install sideko-inc/tap/sideko`).

**Human URL:** [https://github.com/Sideko-Inc/homebrew-tap](https://github.com/Sideko-Inc/homebrew-tap)

## Common Properties

- [Website](https://www.sideko.dev/)
- [Documentation](https://docs.sideko.dev/)
- [Sign Up](https://authentication.sideko.dev/sign-up)
- [Pricing](https://sideko.dev/pricing)
- [Blog & Resources](https://sideko.dev/resources)
- [GitHub Org](https://github.com/Sideko-Inc)
- [ChangeLog](https://docs.sideko.dev/changelog/)
- [Terms of Service](https://www.sideko.dev/legal/terms)
- [Privacy Policy](https://www.sideko.dev/legal/privacy)

## Capabilities

### Workflow Capabilities

- [API Tooling Lifecycle](capabilities/api-tooling-lifecycle.yaml) — Unified workflow that ingests an OpenAPI version, lints it, generates SDKs and an MCP server, deploys mocks, and publishes documentation.

### Per-API Capabilities

- [API Projects](capabilities/sideko-api-projects.yaml)
- [Authentication](capabilities/sideko-authentication.yaml)
- [SDK Generation](capabilities/sideko-sdk-generation.yaml)
- [MCP Generation](capabilities/sideko-mcp-generation.yaml)
- [Documentation](capabilities/sideko-documentation.yaml)
- [Mock Servers](capabilities/sideko-mock-servers.yaml)
- [OpenAPI Linting](capabilities/sideko-linting.yaml)

## Examples

- [List API Projects](examples/sideko-list-api-projects-example.json)
- [Trigger SDK Generation](examples/sideko-trigger-sdk-generation-example.json)
- [Trigger MCP Generation](examples/sideko-trigger-mcp-generation-example.json)
- [Deploy Mock Server](examples/sideko-deploy-mock-server-example.json)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
