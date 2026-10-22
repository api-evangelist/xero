---
generated: '2026-10-20'
method: generated
name: xero-record-and-correct-bank-transactions
description: Record spend or receive money against a Xero bank account, then review and correct the transactions.
api: openapi/xero-accounting-api-openapi.yml
operations:
- getAccounts
- createBankTransactions
- getBankTransactions
- getBankTransaction
- updateBankTransaction
source: Grounded in openapi/xero-accounting-api-openapi.yml. Every operationId was checked against the spec. Auth
  per authentication/xero-authentication.yml; MCP bindings per mcp/xero-tool-crosswalk.yml.
---

# Record and correct bank transactions

Record spend or receive money against a Xero bank account, then review and correct the transactions.

## Auth and headers
- OAuth 2.0 authorization code flow: authorize at `https://login.xero.com/identity/connect/authorize`, exchange the code at `https://identity.xero.com/connect/token` (from the spec's `OAuth2` security scheme; see `authentication/xero-authentication.yml` and `scopes/xero-scopes.yml`).
- Every call needs the `xero-tenant-id` header (the organisation you were granted access to).
- Base URL: `https://api.xero.com/api.xro/2.0`.

## Steps
1. **Pick the bank account**: `getAccounts` (`GET /Accounts`) with `where=Type=="BANK"`. Keep the `AccountID`.
2. **Record transactions**: `createBankTransactions` (`PUT /BankTransactions`) with `Type` (`SPEND` or `RECEIVE`), `BankAccount.AccountID`, `Contact` and `LineItems`.
3. **Review**: `getBankTransactions` (`GET /BankTransactions`), filtered with `where` or `If-Modified-Since`.
4. **Correct one**: `getBankTransaction` (`GET /BankTransactions/{BankTransactionID}`), then `updateBankTransaction` (`POST /BankTransactions/{BankTransactionID}`) with the changed fields.

## Rules
- Create and update operations accept an `Idempotency-Key` header (max 128 characters). Reuse the same key when retrying so a request is not processed twice (marked per operation in `overlays/`).
- The MCP tools `list-bank-transactions`, `create-bank-transaction` and `update-bank-transaction` call these same operations.
