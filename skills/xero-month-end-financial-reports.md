---
generated: '2026-10-20'
method: generated
name: xero-month-end-financial-reports
description: 'Pull the organisation profile and the core month-end reports from Xero: profit and loss, balance sheet,
  trial balance and aged receivables.'
api: openapi/xero-accounting-api-openapi.yml
operations:
- getOrganisations
- getReportProfitAndLoss
- getReportBalanceSheet
- getReportTrialBalance
- getReportAgedReceivablesByContact
- getContacts
source: Grounded in openapi/xero-accounting-api-openapi.yml. Every operationId was checked against the spec. Auth
  per authentication/xero-authentication.yml; MCP bindings per mcp/xero-tool-crosswalk.yml.
---

# Month end financial reports

Pull the organisation profile and the core month-end reports from Xero: profit and loss, balance sheet, trial balance and aged receivables.

## Auth and headers
- OAuth 2.0 authorization code flow: authorize at `https://login.xero.com/identity/connect/authorize`, exchange the code at `https://identity.xero.com/connect/token` (from the spec's `OAuth2` security scheme; see `authentication/xero-authentication.yml` and `scopes/xero-scopes.yml`).
- Every call needs the `xero-tenant-id` header (the organisation you were granted access to).
- Base URL: `https://api.xero.com/api.xro/2.0`.

## Steps
1. **Organisation context**: `getOrganisations` (`GET /Organisation`). Read the base currency and financial year end.
2. **Profit and loss**: `getReportProfitAndLoss` (`GET /Reports/ProfitAndLoss`) with `fromDate`/`toDate`, and optionally `periods` and `timeframe` for comparisons.
3. **Balance sheet**: `getReportBalanceSheet` (`GET /Reports/BalanceSheet`) with `date`.
4. **Trial balance**: `getReportTrialBalance` (`GET /Reports/TrialBalance`) with `date`.
5. **Aged receivables per customer**: find each `ContactID` with `getContacts`, then call `getReportAgedReceivablesByContact` (`GET /Reports/AgedReceivablesByContact`) with `contactId`.

## Rules
- Create and update operations accept an `Idempotency-Key` header (max 128 characters). Reuse the same key when retrying so a request is not processed twice (marked per operation in `overlays/`).
- These are read-only calls, so no idempotency key is needed. The MCP tools `list-organisation-details`, `list-profit-and-loss`, `list-report-balance-sheet`, `list-trial-balance` and `list-aged-receivables-by-contact` call the same operations.
