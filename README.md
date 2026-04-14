# Openapi Naming Guide

This repository defines the preferred naming conventions for **Openapi** across documentation, source code, environment variables, package names, and integrations.

## Official name

The preferred display name is:

**Openapi**

## Why this repository exists

People sometimes refer to the organization in inconsistent ways, such as:

- `OpenAPI`
- `OpenApi`
- `openAPI`
- `OPENAPI`

This guide explains which form to use in each context.

## Naming conventions

### 1. Human-readable text

Use:

- **Openapi**

Examples:

- Openapi organization
- Openapi SDK
- Openapi PHP client

Avoid:

- OpenAPI
- openAPI
- OPENAPI

### 2. GitHub organization and repository names

Use lowercase when required by platform conventions:

- `openapi`
- `openapi/openapi-naming`

### 3. Environment variables

Use uppercase snake case:

- `OPENAPI_API_KEY`
- `OPENAPI_BASE_URL`

Standard variables used across Openapi projects:

**OAuth credentials (token management):**

| Variable | Description |
|---|---|
| `OPENAPI_USERNAME` | Account username (email) |
| `OPENAPI_KEY` | API key |
| `OPENAPI_SANDBOX_KEY` | Sandbox API key |

**Bearer tokens (service API commands):**

| Variable | Description |
|---|---|
| `OPENAPI_TOKEN` | Bearer token for production |
| `OPENAPI_SANDBOX_TOKEN` | Bearer token for sandbox |

### 4. PHP classes

Use PascalCase for class names:

- `OpenapiClient`
- `OpenapiConfig`
- `OpenapiException`

### 5. PHP namespaces

Use PascalCase segments:

- `Openapi\Client`
- `Openapi\Support`

### 6. Variables and function names

Use the naming style required by the language.

#### PHP
- `$openapiClient`
- `$openapiConfig`
- `createOpenapiClient()`

#### JavaScript / TypeScript
- `openapiClient`
- `openapiConfig`
- `createOpenapiClient()`

#### Python
- `openapi_client`
- `openapi_config`
- `create_openapi_client()`

### 7. Constants

Use uppercase snake case:

- `OPENAPI_DEFAULT_TIMEOUT`
- `OPENAPI_API_VERSION`

### 8. Package names

Use lowercase where ecosystem conventions require it:

- `openapi-client`
- `openapi-sdk`
- `openapi-php`

## Quick reference

| Context | Preferred form | Example |
|---|---|---|
| Brand / display name | `Openapi` | Openapi SDK |
| GitHub org / repo | `openapi` | `openapi/openapi-naming` |
| Environment variables | `OPENAPI_*` | `OPENAPI_API_KEY` |
| PHP classes | `Openapi*` | `OpenapiClient` |
| PHP namespaces | `Openapi` | `Openapi\Client` |
| Local variables | language convention | `$openapiClient` |
| Constants | `OPENAPI_*` | `OPENAPI_DEFAULT_TIMEOUT` |

## PHP examples

Preferred:

- `OpenapiClient`
- `OpenapiServiceProvider`
- `Openapi\Http\RequestBuilder`
- `$openapiClient`
- `$openapiApiKey`

Avoid:

- `OpenAPIClient`
- `OpenApiClient`
- `$OpenapiClient`
- `$openAPIClient`

## Forms to avoid

Unless a platform or technical convention requires otherwise, avoid:

- `OpenAPI`
- `openAPI`
- `OPENAPI`

## Rule of thumb

- Use **Openapi** for human-facing text
- Use **openapi** where lowercase identifiers are standard
- Use **OPENAPI** where uppercase constants or environment variables are standard

## Status

This repository is the canonical reference for how the name **Openapi** should be written across contexts.