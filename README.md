# Sideko (sideko)
Sideko is an API tooling generation platform that uses OpenAPI Specifications to create SDKs, documentation sites, CLIs, and mock servers. The platform enables organizations to offer a complete suite of API developer tools without writing code, as Sideko generates the tooling automatically from OpenAPI specs. Sideko serves some of the largest organizations in the world, helping improve API developer experience at scale.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - CLI, Documentation, Mock Servers, Platform, SDKs, API Tooling, SDK Generation

## Timestamps

- **Created:** 2025-01-30
- **Modified:** 2026-05-02

## APIs

### Sideko API
The Sideko REST API enables developers to programmatically manage API projects, generate SDKs in multiple languages, deploy CLI tools, create mock servers, and publish API documentation. The API powers the Sideko platform which transforms OpenAPI specifications into complete developer tooling suites automatically.

**Human URL:** [https://docs.sideko.dev/](https://docs.sideko.dev/)

**Base URL:** https://api.sideko.dev/v1

#### Tags:

 - CLI, Documentation, Mock Servers, Platform, SDKs

#### Properties

- [Documentation](https://docs.sideko.dev/)
- [OpenAPI](openapi/sideko-openapi.yml)
- [SpectralRules](rules/sideko-rules.yml)
- [Capabilities](capabilities/api-tooling-lifecycle.yaml)
- [JSONSchema](json-schema/sideko-api-project-schema.json)
- [JSONSchema](json-schema/sideko-sdk-generation-schema.json)
- [JSONLD](json-ld/sideko-context.jsonld)
- [Vocabulary](vocabulary/sideko-vocabulary.yml)

### Sideko CLI
The Sideko CLI provides command-line access to the Sideko platform, enabling developers to generate SDKs, manage API projects, deploy documentation, and run mock servers from the terminal.

**Human URL:** [https://github.com/Sideko-Inc/sideko](https://github.com/Sideko-Inc/sideko)

#### Tags:

 - CLI, Developer Tools, SDKs

### Sideko Node.js SDK
The Sideko Node.js SDK provides TypeScript and JavaScript bindings for the Sideko API.

**Human URL:** [https://github.com/Sideko-Inc/sideko-node-sdk](https://github.com/Sideko-Inc/sideko-node-sdk)

#### Tags:

 - SDK, Node.js, TypeScript, JavaScript

### Sideko Python SDK
The Sideko Python SDK provides Python bindings for the Sideko API.

**Human URL:** [https://github.com/Sideko-Inc/sideko-python-sdk](https://github.com/Sideko-Inc/sideko-python-sdk)

#### Tags:

 - SDK, Python

## Common Properties

- [Website](https://www.sideko.dev/)
- [Documentation](https://docs.sideko.dev/)
- [Sign Up](https://authentication.sideko.dev/sign-up)
- [Pricing](https://sideko.dev/pricing)
- [Blog](https://www.sideko.dev/blog)
- [GitHub](https://github.com/Sideko-Inc)
- [ChangeLog](https://docs.sideko.dev/changelog/)
- [TermsOfService](https://www.sideko.dev/legal/terms)
- [PrivacyPolicy](https://www.sideko.dev/legal/privacy)

## Capabilities

### Workflow Capabilities

- [API Tooling Lifecycle](capabilities/api-tooling-lifecycle.yaml) — Unified workflow for managing the complete API tooling lifecycle: projects, SDK generation, documentation deployment, and mock servers.

### Shared API Definitions

- [Sideko API](capabilities/shared/sideko-api.yaml) — Per-API shared definition for the Sideko REST API

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
