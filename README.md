# Xero (xero)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
