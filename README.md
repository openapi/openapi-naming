# Openapi Naming Guide

This repository defines the preferred naming conventions for **Openapi** across documentation, source code, environment variables, package names, and integrations.

## Table of contents

- [Official name](#official-name)
- [Why this repository exists](#why-this-repository-exists)
- [Naming conventions](#naming-conventions)
  - [1. Human-readable text](#1-human-readable-text)
  - [2. GitHub organization and repository names](#2-github-organization-and-repository-names)
  - [3. Environment variables](#3-environment-variables)
  - [4. Package names](#4-package-names)
  - [5. Constants](#5-constants)
  - [6. PHP](#6-php)
  - [7. JavaScript / TypeScript](#7-javascript--typescript)
  - [8. Python](#8-python)
  - [9. Go](#9-go)
  - [10. Rust](#10-rust)
- [Quick reference](#quick-reference)
- [Forms to avoid](#forms-to-avoid)
- [Rule of thumb](#rule-of-thumb)

## Official name

The preferred display name is:

**Openapi**

## Why this repository exists

The name is written in one way only:

| | Form |
|---|---|
| ✅ | `Openapi` |
| ❌ | `OpenAPI` |
| ❌ | `OpenApi` |
| ❌ | `openAPI` |
| ❌ | `OPENAPI` |

This guide explains which form to use in each technical context.

## Naming conventions

### 1. Human-readable text

| | Form | Example |
|---|---|---|
| ✅ | `Openapi` | Openapi organization, Openapi SDK |
| ❌ | `OpenAPI` | |
| ❌ | `openAPI` | |
| ❌ | `OPENAPI` | |

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

### 4. Package names

Use lowercase where ecosystem conventions require it:

- `openapi-client`
- `openapi-sdk`
- `openapi-php`

### 5. Constants

Use uppercase snake case:

- `OPENAPI_DEFAULT_TIMEOUT`
- `OPENAPI_API_VERSION`

### 6. PHP

**Classes:** PascalCase prefixed with `Openapi`

- `OpenapiClient`
- `OpenapiConfig`
- `OpenapiException`
- `OpenapiServiceProvider`

**Namespaces:** PascalCase segments

- `Openapi\Client`
- `Openapi\Support`
- `Openapi\Http\RequestBuilder`

**Variables:** camelCase

- `$openapiClient`
- `$openapiConfig`
- `$openapiApiKey`

**Functions:** camelCase

- `createOpenapiClient()`

Avoid: `OpenAPIClient`, `OpenApiClient`, `$OpenapiClient`, `$openAPIClient`

### 7. JavaScript / TypeScript

**Classes:** PascalCase prefixed with `Openapi`

- `OpenapiClient`
- `OpenapiConfig`

**Variables:** camelCase

- `openapiClient`
- `openapiConfig`

**Functions:** camelCase

- `createOpenapiClient()`

### 8. Python

**Classes:** PascalCase prefixed with `Openapi`

- `OpenapiClient`
- `OpenapiConfig`

**Modules:** snake_case

- `openapi_client`
- `openapi_config`

**Variables and functions:** snake_case

- `openapi_client`
- `openapi_config`
- `create_openapi_client()`

### 9. Go

**Types and exported identifiers:** PascalCase prefixed with `Openapi`

- `OpenapiClient`
- `OpenapiConfig`

**Packages:** lowercase

- `openapi`

**Variables:** camelCase

- `openapiClient`
- `openapiConfig`

**Functions:** PascalCase if exported, camelCase if unexported

- `NewOpenapiClient()`
- `newOpenapiClient()`

### 10. Rust

**Structs and enums:** PascalCase prefixed with `Openapi`

- `OpenapiClient`
- `OpenapiConfig`

**Modules and crates:** snake_case

- `openapi_client`
- `openapi_config`

**Variables and functions:** snake_case

- `openapi_client`
- `openapi_config`
- `create_openapi_client()`

## Quick reference

| Context | Preferred form | Example |
|---|---|---|
| Brand / display name | `Openapi` | Openapi SDK |
| GitHub org / repo | `openapi` | `openapi/openapi-naming` |
| Environment variables | `OPENAPI_*` | `OPENAPI_API_KEY` |
| Constants | `OPENAPI_*` | `OPENAPI_DEFAULT_TIMEOUT` |
| PHP / JS / Go classes | `Openapi*` | `OpenapiClient` |
| PHP / Go variables | `$openapiClient` | camelCase |
| Python / Rust variables | `openapi_client` | snake_case |
| Package names | `openapi-*` | `openapi-sdk` |

## Forms to avoid

Unless a platform or technical convention requires otherwise, avoid:

- `OpenAPI`
- `openAPI`
- `openApi`

## Rule of thumb

- Use **Openapi** for human-facing text
- Use **openapi** where lowercase identifiers are standard
- Use **OPENAPI** where uppercase constants or environment variables are standard

## Status

This repository is the canonical reference for how the name **Openapi** should be written across contexts.
