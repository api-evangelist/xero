# Xero GraphQL

## Overview

Xero does not currently offer a public GraphQL API. The Xero developer platform is built entirely on REST, with separate API surface areas for Accounting, Assets, Bank Feeds, Finance, Identity, Payroll (AU/NZ/UK), Projects, and Files. All endpoints are served under `https://api.xero.com` and secured via OAuth 2.0.

A probe against `https://api.xero.com/graphql` returns HTTP 403 Forbidden, confirming no public GraphQL endpoint exists as of June 2026.

## Conceptual Schema

The file `xero-schema.graphql` in this directory is a **conceptual GraphQL schema** derived from the Xero REST API surface. It maps Xero's documented resource types, relationships, enumerations, and query patterns into GraphQL SDL notation. It is not an officially published schema from Xero — it is provided to illustrate how Xero's data model could be represented in GraphQL form for tooling, documentation, and integration planning purposes.

## Source Documentation

- Developer Portal: https://developer.xero.com/
- Accounting API: https://developer.xero.com/documentation/api/accounting/overview
- Assets API: https://developer.xero.com/documentation/api/assets/overview
- Bank Feeds API: https://developer.xero.com/documentation/api/bank-feeds/overview
- Finance API: https://developer.xero.com/documentation/api/finance/overview
- Identity API: https://developer.xero.com/documentation/guides/oauth2/overview/
- Payroll AU API: https://developer.xero.com/documentation/api/payroll-au/overview
- Payroll NZ API: https://developer.xero.com/documentation/api/payroll-nz/overview
- Payroll UK API: https://developer.xero.com/documentation/api/payroll-uk/overview
- Projects API: https://developer.xero.com/documentation/api/projects/overview
- Files API: https://developer.xero.com/documentation/api/files/overview
- GitHub Organisation: https://github.com/XeroAPI

## Notes

- No GraphQL endpoint is available on the Xero platform.
- The schema file in this directory is conceptual and intended for reference only.
- Xero provides OpenAPI 3.0 specifications for all REST APIs in the XeroAPI GitHub organisation.
- Xero provides an MCP server for AI-assisted accounting workflows at https://github.com/XeroAPI/xero-mcp-server.
