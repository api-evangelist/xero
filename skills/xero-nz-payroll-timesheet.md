---
generated: '2026-10-20'
method: generated
name: xero-nz-payroll-timesheet
description: Create a timesheet for a Xero Payroll NZ employee, add lines, and approve it (or revert it to draft).
api: openapi/xero-payrollnz-api-openapi.yml
operations:
- getEmployees
- getPayRunCalendars
- getEarningsRates
- createTimesheet
- createTimesheetLine
- getTimesheet
- approveTimesheet
- revertTimesheet
source: Grounded in openapi/xero-payrollnz-api-openapi.yml. Every operationId was checked against the spec. Auth
  per authentication/xero-authentication.yml; MCP bindings per mcp/xero-tool-crosswalk.yml.
---

# Nz payroll timesheet

Create a timesheet for a Xero Payroll NZ employee, add lines, and approve it (or revert it to draft).

## Auth and headers
- OAuth 2.0 authorization code flow: authorize at `https://login.xero.com/identity/connect/authorize`, exchange the code at `https://identity.xero.com/connect/token` (from the spec's `OAuth2` security scheme; see `authentication/xero-authentication.yml` and `scopes/xero-scopes.yml`).
- Every call needs the `xero-tenant-id` header (the organisation you were granted access to).
- Base URL: `https://api.xero.com/payroll.xro/2.0`.

## Steps
1. **Employee**: `getEmployees` (`GET /Employees`). Keep the `employeeID`.
2. **Pay period**: `getPayRunCalendars` (`GET /PayRunCalendars`). Keep the `payrollCalendarID` and the period dates.
3. **Earnings rate**: `getEarningsRates` (`GET /EarningsRates`). Keep the `earningsRateID` for the timesheet lines.
4. **Create the timesheet**: `createTimesheet` (`POST /Timesheets`) with `payrollCalendarID`, `employeeID`, `startDate`, `endDate` and, optionally, `timesheetLines`.
5. **Add lines**: `createTimesheetLine` (`POST /Timesheets/{TimesheetID}/Lines`) with `date`, `earningsRateID` and `numberOfUnits`.
6. **Approve**: `approveTimesheet` (`POST /Timesheets/{TimesheetID}/Approve`). Check the result with `getTimesheet`. To edit it after approval, call `revertTimesheet` (`POST /Timesheets/{TimesheetID}/RevertToDraft`).

## Rules
- Create and update operations accept an `Idempotency-Key` header (max 128 characters). Reuse the same key when retrying so a request is not processed twice (marked per operation in `overlays/`).
- This covers the NZ Payroll API only. AU and UK payroll have separate specs under `openapi/`. The MCP tools `create-payroll-timesheet`, `add-payroll-timesheet-line`, `approve-payroll-timesheet` and `revert-payroll-timesheet` call these same Payroll NZ operations.
