# Justworks

API Evangelist profile for [Justworks](https://www.justworks.com) — a New York City-based Professional Employer Organization (PEO) and small-business HR platform bundling payroll, tax filing, benefits, 401(k), workers comp, time tracking, and HR consulting into a single per-employee-per-month subscription.

Justworks exposes a [Partner API](https://public-api.justworks.com/v1/docs) at `public-api.justworks.com` for approved integration partners.

## Products

| Product | Starting Price | Description |
| --- | --- | --- |
| **Justworks Payroll** | $8 PEPM | Standalone payroll, tax filing, time tracking, HR tooling — bring your own benefits |
| **Justworks PEO Basic** | $59 PEPM | Co-employment PEO with payroll, compliance, access to large-group benefits |
| **Justworks PEO Plus** | $109 PEPM | PEO Basic plus medical, dental, vision, life/AD&D, disability, and 401(k) admin |
| **Justworks EOR International** | $599 PEPM | Employer of record for full-time employees abroad without a local entity |

## Partner API Surface

| API | Methods | Description |
| --- | --- | --- |
| **Members** | GET | Member profiles, employment history, pay history, custom fields, U.S. tax IDs (SSN) |
| **Company** | GET | Company identity, bank account, business info, custom-field definitions, jurisdictions |
| **Payroll** | GET | Payroll runs, per-payroll fees, paystubs (earnings + deductions + employer contributions) |
| **Deductions** | GET / POST / PUT / PATCH | List, create, update, cancel deductions with per-row operation_id idempotency — primary write surface |
| **Time Off** | GET / POST | Asynchronous balance reports, policies, requests |
| **Webhooks** | POST | List, resume, simulate signed at-least-once webhooks |
| **OAuth** | POST | Authorization code + refresh token + revoke |

**Auth:** OAuth 2.0 authorization code flow. Access tokens valid 24h, refresh tokens valid 30d. Scopes are hierarchical (e.g., `member.detail:read` implies `member.basic:read` implies `member.dob:read` and `member.sex:read`).

**Webhook events:** `member.profile.created`, `member.profile.updated`, `member.employment_state.termination_scheduled`, `member.employment_state.termination_canceled`, `department.created`, `department.updated`, `department.deleted`.

**Conventions:** Cursor pagination with `limit` cap of 100, monetary fields as zero-decimal integers (e.g., `$45.00` is `4500`), `updated_at` filters support `_gt`, `_gte`, `_lt`, `_lte`, `_ne` operators.

## Artifacts

| Folder | Files |
| --- | --- |
| [`openapi/`](openapi/) | 7 OpenAPI 3.1 specs covering every Partner API endpoint |
| [`capabilities/`](capabilities/) | 6 Naftiko capability files exposing each API surface as MCP tools |
| [`json-schema/`](json-schema/) | 6 JSON Schemas for Member, Company, Payroll, Paystub, Deduction, Time Off Request, Webhook Event |
| [`json-ld/`](json-ld/) | JSON-LD context aligning Justworks resources with schema.org Person, Organization, Salary, and Dates |
| [`plans/`](plans/) | API Commons Plans 0.1 file capturing the four subscription tiers + free Partner API access |
| [`rate-limits/`](rate-limits/) | API Commons Rate Limits 0.1 file capturing cursor caps, token TTLs, and webhook delivery semantics |
| [`finops/`](finops/) | FOCUS-aligned FinOps view of per-seat, per-payroll-run, and benefits-premium charges |

## Integrations

Justworks publishes a partner [integration marketplace](https://www.justworks.com/integrations) including Greenhouse, Lever, JazzHR (hiring), CultureAmp and 15Five (performance), QuickBooks, NetSuite, Xero, and Sage Intacct (accounting), and Brex and Ramp (expense). Justworks also flows through HRIS aggregators including [Finch](https://www.tryfinch.com/integrations/justworks), [Merge](https://www.merge.dev/integrations/justworks), and [Apideck](https://developers.apideck.com/apis/hris/justworks).

## Links

- Website: https://www.justworks.com
- Partner API docs: https://public-api.justworks.com/v1/docs
- Partner program: https://www.justworks.com/partners
- Pricing: https://www.justworks.com/pricing
- Help center: https://help.justworks.com
- Trust center: https://trust.justworks.com
- GitHub: https://github.com/justworkshr
