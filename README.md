# Justworks (justworks)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Justworks is a New York City-based Professional Employer Organization (PEO) and small-business HR
platform. It bundles payroll, tax filing, multi-state compliance, large-group medical/dental/vision
benefits, 401(k) administration, workers comp, time tracking, and HR consulting into a single
per-employee-per-month subscription. Justworks operates four primary products: Justworks Payroll
(standalone payroll), Justworks PEO Basic, Justworks PEO Plus (PEO with included benefits package),
and Justworks EOR International for hiring full-time employees abroad without a local entity.

Justworks exposes a Partner API at public-api.justworks.com for approved integration partners,
covering Members, Company, Payroll, Paystubs, Deductions, Time Off, and Webhooks. The API uses OAuth
2.0 authorization-code grant, cursor pagination, signed at-least-once webhooks, and zero-decimal
currency representation. Deductions is the primary write surface; everything else is read-only.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- PEO
- Payroll
- HR
- Human Resources
- Benefits
- Health Insurance
- 401(k)
- Time Off
- Compliance
- Small Business
- Employer of Record
- HRIS

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Justworks Members API

Read employee, contractor, and member information from the Justworks Partner API. Provides access to
member profiles, employment history, pay history, custom-field values, and U.S. tax identifiers
(SSN) for domestic members. This is the canonical workforce-truth surface a partner integrates
against. Uses cursor pagination with a hard cap of 100 items per page.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- HR
- PEO
- Members
- Employees

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-members-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-members-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-members-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/justworks-member-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/justworks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Justworks Company API

Read company-level data from the Justworks Partner API including company identity, departments,
offices, bank account on file (masked), verified business information, custom-field definitions,
and the jurisdictions in which the company operates.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- HR
- PEO
- Company

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-company-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-company-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-company-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Justworks Payroll API

Read payroll runs, fees, and paystubs. Each payroll record summarizes gross pay, net pay, employee
and employer taxes, and debit information; paystubs break down per-member earnings, employee
deductions, and employer contributions. Monetary fields are zero-decimal integers.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- Payroll
- PEO
- Paystubs

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-payroll-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-payroll-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-payroll-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/justworks-payroll-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/justworks-paystub-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Justworks Deductions API

Manage employee deductions — list deduction types, create one-time and recurring deductions,
update existing deductions, and cancel deductions in bulk. The primary write surface of the
Justworks Partner API. Each item carries a partner-supplied operation_id for idempotency.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- Deductions
- Payroll
- PEO

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-deductions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-deductions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-deductions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/justworks-deduction-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Justworks Time Off API

Manage time-off balances, policies, and requests. Balance reports are asynchronous — submit a
POST, then poll the report endpoint until ready. Policies and requests are paginated reads with
standard cursor semantics.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- Time Off
- PTO
- Leave
- HR

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-time-off-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-time-off-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-time-off-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/justworks-time-off-request-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Justworks Webhooks API

Manage Justworks Partner API webhooks. Justworks signs every request, delivers events at-least-once
with automatic retries, and closes a webhook on sustained failures (resumable via API). Event types
cover member.profile.*, member.employment_state.termination_*, and department.* lifecycle changes.
A Tour-environment simulate endpoint allows partners to validate their listener without real data.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- Webhooks
- Events
- HR

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-webhooks-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-webhooks-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-webhooks-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/justworks-webhook-event-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Justworks OAuth API

OAuth 2.0 token endpoints for the Justworks Partner API. Authorization code is the only supported
grant for initial token acquisition; refresh token grant is supported for renewal. Access tokens are
valid for 24 hours; refresh tokens are valid for 30 days. A revoke endpoint is provided for both
access and refresh tokens.

- **Human URL:** [https://public-api.justworks.com/v1/docs](https://public-api.justworks.com/v1/docs)

#### Tags

- OAuth
- Authentication

#### Properties

- [Documentation](https://public-api.justworks.com/v1/docs)
- [OpenAPI](openapi/justworks-oauth-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/justworks-oauth-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/justworks-oauth-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.justworks.com)
- [Documentation](https://public-api.justworks.com/v1/docs)
- [Portal](https://www.justworks.com/partners)
- [Getting Started](https://public-api.justworks.com/v1/docs)
- [Pricing](https://www.justworks.com/pricing)
- [Products](https://www.justworks.com/products)
- [Integrations](https://www.justworks.com/integrations)
- [Partner Program](https://www.justworks.com/partners)
- [Partner Integrations](https://www.justworks.com/partners/integrations)
- [Partner Blog](https://www.justworks.com/partners/blog)
- [Help Center](https://help.justworks.com)
- [Trust Center](https://trust.justworks.com)
- [Blog](https://www.justworks.com/blog)
- [Careers](https://www.justworks.com/careers)
- [GitHub Organization](https://github.com/justworkshr)
- [LinkedIn](https://www.linkedin.com/company/justworks)
- [Twitter](https://twitter.com/JustworksHR)
- [YouTube](https://www.youtube.com/c/Justworks)
- [Plans](plans/justworks-plans-pricing.yml)
- [Rate Limits](rate-limits/justworks-rate-limits.yml)
- [Fin Ops](finops/justworks-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
