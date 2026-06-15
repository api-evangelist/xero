# Xero (xero)

Xero is a cloud-based accounting software platform that helps small and medium-sized businesses manage their finances. Xero provides a comprehensive developer platform with OAuth 2.0 APIs for accounting, payroll, assets, projects, files, bank feeds, and identity management. The Xero API enables third-party integrations to build custom accounting apps, automations, and business tools. Xero supports SDKs for .NET, Java, Node.js, PHP, Ruby, Python, and provides an MCP server for AI-assisted accounting workflows.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/apis.yml)

## Tags

- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business

## Timestamps

- **Created:** 2024-11-07
- **Modified:** 2026-05-30

## APIs

### Xero Accounting API

Core accounting API for the Xero platform. Supports creating and managing accounts, invoices, credit notes, bank transactions, contacts, payments, purchase orders, and financial reports. Provides comprehensive access to all accounting functions in Xero including chart of accounts, journal entries, tax rates, currencies, and tracking categories.

- **Human URL:** [https://developer.xero.com/documentation/api/accounting/overview](https://developer.xero.com/documentation/api/accounting/overview)
- **Base URL:** `https://api.xero.com/api.xro/2.0`

#### Tags

- Accounting
- Finance
- Invoicing

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/accounting/overview)
- [OpenAPI](openapi/xero-accounting-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-accounting.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-accounting.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/xero-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Xero Assets API

API for managing fixed assets in Xero. Supports registering and depreciating assets, managing asset types, and running depreciation calculations. Enables automated fixed asset lifecycle management integrated with Xero accounting.

- **Human URL:** [https://developer.xero.com/documentation/api/assets/overview](https://developer.xero.com/documentation/api/assets/overview)
- **Base URL:** `https://api.xero.com/assets.xro/1.0`

#### Tags

- Assets
- Depreciation
- Finance

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/assets/overview)
- [OpenAPI](openapi/xero-assets-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-assets.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-assets.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Bank Feeds API

API for importing bank transaction data into Xero from financial institutions and fintech providers. Enables creation and management of bank feed connections and statement lines for automated bank reconciliation workflows.

- **Human URL:** [https://developer.xero.com/documentation/api/bank-feeds/overview](https://developer.xero.com/documentation/api/bank-feeds/overview)
- **Base URL:** `https://api.xero.com/bankfeeds.xro/1.0`

#### Tags

- Bank Feeds
- Banking
- Reconciliation

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/bank-feeds/overview)
- [OpenAPI](openapi/xero-bankfeeds-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-bankfeeds.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-bankfeeds.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Finance API

API providing access to financial statements, balance sheets, profit and loss reports, and cash flow summaries for Xero organizations. Supports bank statement accounting, account usage, and lock history for financial analysis and reporting applications.

- **Human URL:** [https://developer.xero.com/documentation/api/finance/overview](https://developer.xero.com/documentation/api/finance/overview)
- **Base URL:** `https://api.xero.com/finance.xro/1.0`

#### Tags

- Finance
- Financial Reporting
- Reports

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/finance/overview)
- [OpenAPI](openapi/xero-finance-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-finance.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-finance.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Identity API

OAuth 2.0 authentication and authorization API for the Xero platform. Manages connections to Xero organizations, user identity, and refresh token lifecycle. Required for all Xero API integrations to obtain and manage access tokens.

- **Human URL:** [https://developer.xero.com/documentation/guides/oauth2/overview/](https://developer.xero.com/documentation/guides/oauth2/overview/)
- **Base URL:** `https://identity.xero.com`

#### Tags

- Authentication
- Identity
- OAuth 2.0

#### Properties

- [Documentation](https://developer.xero.com/documentation/guides/oauth2/overview/)
- [OpenAPI](openapi/xero-identity-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-identity.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-identity.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Payroll Australia API

Payroll management API for Australian businesses using Xero. Supports managing employees, pay runs, pay slips, leave applications, payroll calendars, tax declarations, and superannuation. Compliant with Australian payroll regulations including Single Touch Payroll (STP).

- **Human URL:** [https://developer.xero.com/documentation/api/payroll-au/overview](https://developer.xero.com/documentation/api/payroll-au/overview)
- **Base URL:** `https://api.xero.com/payroll.xro/1.0`

#### Tags

- Australia
- Payroll
- Superannuation

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/payroll-au/overview)
- [OpenAPI](openapi/xero-payroll-au-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-payroll-au.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-payroll-au.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Payroll New Zealand API

Payroll management API for New Zealand businesses using Xero. Supports managing employees, pay runs, pay slips, leave management, and compliance with New Zealand payroll regulations including KiwiSaver and PAYE.

- **Human URL:** [https://developer.xero.com/documentation/api/payroll-nz/overview](https://developer.xero.com/documentation/api/payroll-nz/overview)
- **Base URL:** `https://api.xero.com/payroll.xro/1.0`

#### Tags

- New Zealand
- Payroll

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/payroll-nz/overview)
- [OpenAPI](openapi/xero-payroll-nz-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-payroll-nz.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-payroll-nz.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Payroll United Kingdom API

Payroll management API for UK businesses using Xero. Supports managing employees, pay runs, pay slips, leave, and compliance with UK payroll regulations including PAYE, national insurance, pensions, and Real Time Information (RTI) submissions to HMRC.

- **Human URL:** [https://developer.xero.com/documentation/api/payroll-uk/overview](https://developer.xero.com/documentation/api/payroll-uk/overview)
- **Base URL:** `https://api.xero.com/payroll.xro/1.0`

#### Tags

- Payroll
- United Kingdom

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/payroll-uk/overview)
- [OpenAPI](openapi/xero-payroll-uk-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-payroll-uk.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-payroll-uk.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Projects API

Project tracking and time management API for Xero. Supports creating and managing projects, tasks, time entries, and expenses. Enables integration of project-based billing with Xero accounting for professional services and project-based businesses.

- **Human URL:** [https://developer.xero.com/documentation/api/projects/overview](https://developer.xero.com/documentation/api/projects/overview)
- **Base URL:** `https://api.xero.com/projects.xro/2.0`

#### Tags

- Projects
- Time Tracking

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/projects/overview)
- [OpenAPI](openapi/xero-projects-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-projects.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-projects.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Xero Files API

File storage and management API for Xero. Supports uploading, organizing, and attaching files to accounting objects in Xero. Enables document management workflows integrated with accounting records for invoices, receipts, and other financial documents.

- **Human URL:** [https://developer.xero.com/documentation/api/files/overview](https://developer.xero.com/documentation/api/files/overview)
- **Base URL:** `https://api.xero.com/files.xro/1.0`

#### Tags

- Documents
- Files
- Storage

#### Properties

- [Documentation](https://developer.xero.com/documentation/api/files/overview)
- [OpenAPI](openapi/xero-files-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/xero-files.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/xero-files.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/xero)
- [Portal](https://developer.xero.com/)
- [Documentation](https://developer.xero.com/documentation/)
- [Getting Started](https://developer.xero.com/documentation/getting-started-guide/)
- [Authentication](https://developer.xero.com/documentation/guides/oauth2/overview/)
- [S D Ks](https://developer.xero.com/documentation/sdks-and-tools/libraries/overview/)
- [Webhooks](https://developer.xero.com/documentation/guides/webhooks/overview/)
- [Changelog](https://developer.xero.com/changelog)
- [Blog](https://devblog.xero.com/)
- [F A Q](https://developer.xero.com/faq)
- [Terms of Service](https://developer.xero.com/xero-developer-platform-terms-conditions/)
- [Privacy Policy](https://www.xero.com/us/legal/privacy/)
- [Status Page](https://status.xero.com/)
- [Sign Up](https://www.xero.com/us/signup/developers/)
- [GitHub Organization](https://github.com/XeroAPI)
- [M C P Server](https://github.com/XeroAPI/xero-mcp-server)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
