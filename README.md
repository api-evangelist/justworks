# Justworks

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

**Areas:** PEO · Payroll · Human Resources · Benefits · Health Insurance · 401k · Time Off · Compliance · Small Business · Employer of Record · HRIS · Employee Benefits

## Justworks on APIs.io

Everything profiled for Justworks is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/justworks/](https://apis.io/providers/justworks/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Justworks Members API](https://apis.io/apis/justworks/justworks-members-api/) — Read employee, contractor, and member information from the Justworks Partner API. Provides access to member profiles, employment history, pay history,…
- [Justworks Company API](https://apis.io/apis/justworks/justworks-company-api/) — Read company-level data from the Justworks Partner API including company identity, departments, offices, bank account on file (masked), verified business…
- [Justworks Deductions API](https://apis.io/apis/justworks/justworks-deductions-api/) — Manage employee deductions — list deduction types, create one-time and recurring deductions, update existing deductions, and cancel deductions in bulk. The…
- [Justworks Webhooks API](https://apis.io/apis/justworks/justworks-webhooks-api/) — Manage Justworks Partner API webhooks. Justworks signs every request, delivers events at-least-once with automatic retries, and closes a webhook on…
- [Justworks Deduction Types API](https://apis.io/apis/justworks/justworks-deduction-types-api/) — Read access to Justworks deduction type catalog
- [Justworks Payrolls API](https://apis.io/apis/justworks/justworks-payrolls-api/) — Read access to payroll runs and per-payroll fees
- [Justworks Paystubs API](https://apis.io/apis/justworks/justworks-paystubs-api/) — Read access to per-member paystubs
- [Justworks Time Off Balances API](https://apis.io/apis/justworks/justworks-time-off-balances-api/) — Asynchronous balance reports for time-off policies
- [Justworks Time Off Policies API](https://apis.io/apis/justworks/justworks-time-off-policies-api/) — Read access to time-off policy catalog
- [Justworks Time Off Requests API](https://apis.io/apis/justworks/justworks-time-off-requests-api/) — Read access to time-off requests submitted by members
- [Justworks O Auth API](https://apis.io/apis/justworks/justworks-oauth-api/) — OAuth 2.0 token endpoints

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [justworks](https://apis.io/servers/justworks/justworks/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Justworks Agentic Access](https://apis.io/agentic-access/justworks/justworks-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [Justworks Deduction](https://apis.io/schemas/justworks/justworks-deduction/)
- [Justworks Member](https://apis.io/schemas/justworks/justworks-member/)
- [Justworks Payroll](https://apis.io/schemas/justworks/justworks-payroll/)
- [Justworks Paystub](https://apis.io/schemas/justworks/justworks-paystub/)
- [Justworks Time Off Request](https://apis.io/schemas/justworks/justworks-time-off-request/)
- [Justworks Webhook Event](https://apis.io/schemas/justworks/justworks-webhook-event/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Justworks Context](https://apis.io/jsonld/justworks/justworks-context/)

#### Collections (13)

Postman and Open Collection request collections.

- [Justworks Company API](https://apis.io/collections/justworks/open-justworks-company-api/)
- [Justworks Company Deduction Types API](https://apis.io/collections/justworks/open-justworks-deduction-types-api/)
- [Justworks Company Deductions API](https://apis.io/collections/justworks/open-justworks-deductions-api/)
- [Justworks Company Members API](https://apis.io/collections/justworks/open-justworks-members-api/)
- [Justworks Company OAuth API](https://apis.io/collections/justworks/open-justworks-oauth-api/)
- [Justworks Payroll API](https://apis.io/collections/justworks/open-justworks-payroll-api/)
- [Justworks Company Payrolls API](https://apis.io/collections/justworks/open-justworks-payrolls-api/)
- [Justworks Company Paystubs API](https://apis.io/collections/justworks/open-justworks-paystubs-api/)
- [Justworks Time Off API](https://apis.io/collections/justworks/open-justworks-time-off-api/)
- [Justworks Company Time Off Balances API](https://apis.io/collections/justworks/open-justworks-time-off-balances-api/)
- [Justworks Company Time Off Policies API](https://apis.io/collections/justworks/open-justworks-time-off-policies-api/)
- [Justworks Company Time Off Requests API](https://apis.io/collections/justworks/open-justworks-time-off-requests-api/)
- [Justworks Company Webhooks API](https://apis.io/collections/justworks/open-justworks-webhooks-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Justworks — jsonschema rules](https://apis.io/rules/justworks/justworks-jsonschema-spectral-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Justworks Authentication](https://apis.io/security/justworks/justworks-authentication/)
- [Justworks Domain Security](https://apis.io/security/justworks/justworks-domain-security/)
- [Justworks Vulnerability Disclosure](https://apis.io/security/justworks/justworks-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Justworks Scopes](https://apis.io/scopes/justworks/justworks-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Justworks Plans Pricing](https://apis.io/plans/justworks/justworks-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Justworks Rate Limits](https://apis.io/rate-limits/justworks/justworks-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Justworks Finops](https://apis.io/finops/justworks/justworks-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.justworks.com)
- [Documentation](https://public-api.justworks.com/v1/docs)
- [Getting started](https://public-api.justworks.com/v1/docs)
- [Pricing](https://www.justworks.com/pricing)
- [Blog](https://www.justworks.com/blog)
- [Trust centre](https://trust.justworks.com)
- [GitHub](https://github.com/justworkshr)

## API Evangelist rating

**Kin Score 42.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 60.0 |
| Contract quality | 58.9 |
| Contract governance | 9.8 |
| Operational transparency | 18.4 |
| Developer ergonomics | 51.2 |
| Access clarity | 30.3 |

**Agent readiness 41.7** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 34.8** — Employment & Payroll

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/justworks/](https://apis.io/providers/justworks/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Justworks: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/justworks/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
