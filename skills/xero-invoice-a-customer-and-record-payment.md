---
generated: '2026-10-20'
method: generated
name: xero-invoice-a-customer-and-record-payment
description: Find or create a contact in Xero, raise a sales invoice for it, email it, and record the payment against
  it.
api: openapi/xero-accounting-api-openapi.yml
operations:
- getContacts
- createContacts
- createInvoices
- emailInvoice
- getInvoice
- createPayment
source: Grounded in openapi/xero-accounting-api-openapi.yml. Every operationId was checked against the spec. Auth
  per authentication/xero-authentication.yml; MCP bindings per mcp/xero-tool-crosswalk.yml.
---

# Invoice a customer and record payment

Find or create a contact in Xero, raise a sales invoice for it, email it, and record the payment against it.

## Auth and headers
- OAuth 2.0 authorization code flow: authorize at `https://login.xero.com/identity/connect/authorize`, exchange the code at `https://identity.xero.com/connect/token` (from the spec's `OAuth2` security scheme; see `authentication/xero-authentication.yml` and `scopes/xero-scopes.yml`).
- Every call needs the `xero-tenant-id` header (the organisation you were granted access to).
- Base URL: `https://api.xero.com/api.xro/2.0`.

## Steps
1. **Find the customer**: `getContacts` (`GET /Contacts`). Filter with `searchTerm` or `where`. Keep the `ContactID`.
2. **Create the contact if it is missing**: `createContacts` (`PUT /Contacts`) with a `Contacts` array.
3. **Raise the invoice**: `createInvoices` (`PUT /Invoices`) with `Type: ACCREC`, the `Contact.ContactID`, `LineItems` (with `AccountCode` and `TaxType`) and `Status` (`DRAFT` or `AUTHORISED`). Keep the `InvoiceID`.
4. **Email it** (optional, only for authorised invoices): `emailInvoice` (`POST /Invoices/{InvoiceID}/Email`).
5. **Record the payment**: `createPayment` (`POST /Payments`) with `Invoice.InvoiceID`, `Account` (a bank account from `getAccounts`), `Amount` and `Date`.
6. **Confirm**: `getInvoice` (`GET /Invoices/{InvoiceID}`) and check `AmountDue` and `Status` (`PAID` once settled).

## Rules
- Create and update operations accept an `Idempotency-Key` header (max 128 characters). Reuse the same key when retrying so a request is not processed twice (marked per operation in `overlays/`).
- The official Xero MCP tools `list-contacts`, `create-contact`, `create-invoice` and `create-payment` call these same operations (see `mcp/xero-tool-crosswalk.yml`).
