# Workday Business Processes

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

Workday Business Processes is the workflow engine at the centre of Workday HCM and Financial Management: every hire, job change, expense report, requisition and payment runs as a business process event routed through configured approval, to-do and questionnaire steps. Workday exposes it as a first-party REST service, businessProcess v1, which reads business process types, events and event steps and performs the real actions on them — approve, deny, send back, reassign, cancel and rescind — alongside a Custom Business Process Config v1 service for authoring custom process types and event task definitions, business-process operations inside the Integrations SOAP service, and business process query fields in the Workday Graph API.

**Areas:** Business Processes · Workflows · Approvals · Human Resources · Enterprise · Software-as-a-Service · HCM · Financial Management · Process Automation · Event Steps · SOAP · GraphQL

## Workday Business Processes on APIs.io

Everything profiled for Workday Business Processes is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/workday-business-processes/](https://apis.io/providers/workday-business-processes/)** — or go straight to one of the APIs or properties below.

### APIs (30)

- [Workday Integrations SOAP Service (business process operations)](https://apis.io/apis/workday-business-processes/workday-business-processes-integrations-soap-service/) — The Workday Web Services Integrations service, v47.0. Carries the eight SOAP business process operations — Approve, Cancel, Deny, Rescind and Send Back a…
- [Workday Business Processes 03/11/2023 API](https://apis.io/apis/workday-business-processes/workday-business-processes-03-11-2023-api/) — Changes for v2023.10
- [Workday Business Processes 03/15/2021 API](https://apis.io/apis/workday-business-processes/workday-business-processes-03-15-2021-api/) — Changes for v2021.13
- [Workday Business Processes 03/18/2026 API](https://apis.io/apis/workday-business-processes/workday-business-processes-03-18-2026-api/) — Changes for v2026.11
- [Workday Business Processes 04/01/2023 API](https://apis.io/apis/workday-business-processes/workday-business-processes-04-01-2023-api/) — Changes for v2023.13
- [Workday Business Processes 04/02/2022 API](https://apis.io/apis/workday-business-processes/workday-business-processes-04-02-2022-api/) — Changes for v2022.14
- [Workday Business Processes 04/24/2023 API](https://apis.io/apis/workday-business-processes/workday-business-processes-04-24-2023-api/) — Changes for v2023.16
- [Workday Business Processes 05/17/2025 API](https://apis.io/apis/workday-business-processes/workday-business-processes-05-17-2025-api/) — Changes for v2025.20
- [Workday Business Processes 06/08/2026 API](https://apis.io/apis/workday-business-processes/workday-business-processes-06-08-2026-api/) — Changes for v2026.23
- [Workday Business Processes 06/15/2024 API](https://apis.io/apis/workday-business-processes/workday-business-processes-06-15-2024-api/) — Changes for v2024.24
- [Workday Business Processes 06/15/2026 API](https://apis.io/apis/workday-business-processes/workday-business-processes-06-15-2026-api/) — Changes for v2026.24
- [Workday Business Processes 06/30/2026 API](https://apis.io/apis/workday-business-processes/workday-business-processes-06-30-2026-api/) — Changes for v2026.26
- [Workday Business Processes 07/15/2023 API](https://apis.io/apis/workday-business-processes/workday-business-processes-07-15-2023-api/) — Changes for v2023.28
- [Workday Business Processes 08/06/2022 API](https://apis.io/apis/workday-business-processes/workday-business-processes-08-06-2022-api/) — Changes for v2022.32
- [Workday Business Processes 08/17/2026 API](https://apis.io/apis/workday-business-processes/workday-business-processes-08-17-2026-api/) — Changes for v2026.33
- [Workday Business Processes 09/01/2021 API](https://apis.io/apis/workday-business-processes/workday-business-processes-09-01-2021-api/) — Changes for v2021.37
- [Workday Business Processes 09/09/2021 API](https://apis.io/apis/workday-business-processes/workday-business-processes-09-09-2021-api/) — Changes for v2021.38
- [Workday Business Processes 09/19/2022 API](https://apis.io/apis/workday-business-processes/workday-business-processes-09-19-2022-api/) — Changes for v2022.38
- [Workday Business Processes 09/28/2024 API](https://apis.io/apis/workday-business-processes/workday-business-processes-09-28-2024-api/) — Changes for v2024.39
- [Workday Business Processes 12/06/2025 API](https://apis.io/apis/workday-business-processes/workday-business-processes-12-06-2025-api/) — Changes for v2025.49
- [Workday Business Processes 12/15/2025 API](https://apis.io/apis/workday-business-processes/workday-business-processes-12-15-2025-api/) — Changes for v2025.50
- [Workday Business Processes Approvals API](https://apis.io/apis/workday-business-processes/workday-business-processes-approvals-api/) — Manage approval steps and approval chains
- [Workday Business Processes Business Process Definitions API](https://apis.io/apis/workday-business-processes/workday-business-processes-business-process-definitions-api/) — Retrieve and manage business process type definitions
- [Workday Business Processes Event Task Definitions API](https://apis.io/apis/workday-business-processes/workday-business-processes-event-task-definitions-api/) — A collection of Event Task Definitions for custom business process defined in Workday.
- [Workday Business Processes Events API](https://apis.io/apis/workday-business-processes/workday-business-processes-events-api/) — Returns a collection of events based on the specified parameters. You must specify either the worker or initiating worker query parameter. If you did not…
- [Workday Business Processes Event Steps API](https://apis.io/apis/workday-business-processes/workday-business-processes-eventsteps-api/) — Returns a collection of business process event steps based on the specified parameters. Only event steps that are awaiting action from the processing person…
- [Workday Business Processes Inbox Items API](https://apis.io/apis/workday-business-processes/workday-business-processes-inbox-items-api/) — Manage user inbox items requiring action
- [Workday Business Processes Process Instances API](https://apis.io/apis/workday-business-processes/workday-business-processes-process-instances-api/) — Manage running business process instances
- [Workday Business Processes Prompt Values API](https://apis.io/apis/workday-business-processes/workday-business-processes-prompt-values-api/) — Retrieves instances that can be used as values for other endpoint parameters in this service.
- [Workday Business Processes Types API](https://apis.io/apis/workday-business-processes/workday-business-processes-types-api/) — Returns all business process types. Secured by Public Business Processes.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [workday-business-process](https://apis.io/servers/workday-business-processes/workday-business-process/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Workday Business Processes Agentic Access](https://apis.io/agentic-access/workday-business-processes/workday-business-processes-agentic-access/)

#### JSON Schema (7)

The data models the API reads and writes.

- [Approval Request](https://apis.io/schemas/workday-business-processes/workday-business-processes-approval-request/)
- [Business Process Definition](https://apis.io/schemas/workday-business-processes/workday-business-processes-business-process-definition/)
- [Denial Request](https://apis.io/schemas/workday-business-processes/workday-business-processes-denial-request/)
- [Inbox Item](https://apis.io/schemas/workday-business-processes/workday-business-processes-inbox-item/)
- [Initiate Process Request](https://apis.io/schemas/workday-business-processes/workday-business-processes-initiate-process-request/)
- [Process Instance](https://apis.io/schemas/workday-business-processes/workday-business-processes-process-instance/)
- [Process Step](https://apis.io/schemas/workday-business-processes/workday-business-processes-process-step/)

#### JSON Structure (7)

Data models expressed in JSON Structure.

- [Workday Business Processes Approval Request Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-approval-request-structure/)
- [Workday Business Processes Business Process Definition Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-business-process-definition-structure/)
- [Workday Business Processes Denial Request Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-denial-request-structure/)
- [Workday Business Processes Inbox Item Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-inbox-item-structure/)
- [Workday Business Processes Initiate Process Request Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-initiate-process-request-structure/)
- [Workday Business Processes Process Instance Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-process-instance-structure/)
- [Workday Business Processes Process Step Structure](https://apis.io/json-structure/workday-business-processes/workday-business-processes-process-step-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Workday Business Processes Context](https://apis.io/jsonld/workday-business-processes/workday-business-processes-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Workday Business Processes Vocabulary](https://apis.io/vocabularies/workday-business-processes/workday-business-processes-vocabulary/)

#### Examples (7)

Example requests and responses.

- [Workday Business Processes Approval Request Example](https://apis.io/examples/workday-business-processes/workday-business-processes-approval-request-example/)
- [Workday Business Processes Business Process Definition Example](https://apis.io/examples/workday-business-processes/workday-business-processes-business-process-definition-example/)
- [Workday Business Processes Denial Request Example](https://apis.io/examples/workday-business-processes/workday-business-processes-denial-request-example/)
- [Workday Business Processes Inbox Item Example](https://apis.io/examples/workday-business-processes/workday-business-processes-inbox-item-example/)
- [Workday Business Processes Initiate Process Request Example](https://apis.io/examples/workday-business-processes/workday-business-processes-initiate-process-request-example/)
- [Workday Business Processes Process Instance Example](https://apis.io/examples/workday-business-processes/workday-business-processes-process-instance-example/)
- [Workday Business Processes Process Step Example](https://apis.io/examples/workday-business-processes/workday-business-processes-process-step-example/)

#### Collections (9)

Postman and Open Collection request collections.

- [Workday Business Process API](https://apis.io/collections/workday-business-processes/open-workday-business-processes/)
- [Workday Business Process Approvals API](https://apis.io/collections/workday-business-processes/open-workday-business-processes-approvals-api/)
- [Workday Business Process Approvals Business Process Definitions API](https://apis.io/collections/workday-business-processes/open-workday-business-processes-business-process-definitions-api/)
- [Workday Business Process Approvals Inbox Items API](https://apis.io/collections/workday-business-processes/open-workday-business-processes-inbox-items-api/)
- [Workday Business Process Approvals Process Instances API](https://apis.io/collections/workday-business-processes/open-workday-business-processes-process-instances-api/)
- [Workday Business Process Approvals API](https://apis.io/collections/workday-business-processes/postman-workday-business-processes-approvals-api/)
- [Workday Business Process Approvals Business Process Definitions API](https://apis.io/collections/workday-business-processes/postman-workday-business-processes-business-process-definitions-api/)
- [Workday Business Process Approvals Inbox Items API](https://apis.io/collections/workday-business-processes/postman-workday-business-processes-inbox-items-api/)
- [Workday Business Process Approvals Process Instances API](https://apis.io/collections/workday-business-processes/postman-workday-business-processes-process-instances-api/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Workday Business Processes Business Process Overlay](https://apis.io/overlays/workday-business-processes/workday-business-processes-business-process-overlay/)
- [Workday Business Processes Custom Business Process Config Overlay](https://apis.io/overlays/workday-business-processes/workday-business-processes-custom-business-process-config-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Workday Business Processes — jsonschema rules](https://apis.io/rules/workday-business-processes/workday-business-processes-jsonschema-spectral-rules/)
- [Workday Business Processes API Rules](https://apis.io/rules/workday-business-processes/workday-business-processes-spectral-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Workday Business Processes Authentication](https://apis.io/security/workday-business-processes/workday-business-processes-authentication/)
- [Workday Business Processes Domain Security](https://apis.io/security/workday-business-processes/workday-business-processes-domain-security/)
- [Workday Business Processes Trust Center](https://apis.io/security/workday-business-processes/workday-business-processes-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Workday Business Processes Scopes](https://apis.io/scopes/workday-business-processes/workday-business-processes-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Workday Business Processes Plans Pricing](https://apis.io/plans/workday-business-processes/workday-business-processes-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Workday Business Processes Rate Limits](https://apis.io/rate-limits/workday-business-processes/workday-business-processes-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Workday Business Processes Finops](https://apis.io/finops/workday-business-processes/workday-business-processes-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.workday.com/)
- [Documentation](https://developer.workday.com/doc/GUID-e31b535f-7722-4f61-9795-a27ef9d78a86-enHYPHENus.md)
- [Getting started](https://developer.workday.com/doc/zwx1518028675482.md)
- [API reference](https://community.workday.com/sites/default/files/file-hosting/restapi/index.html)
- [Sign up](https://developer.workday.com/login)
- [Support](https://community.workday.com)
- [Blog](https://blog.workday.com/en-us/homepage.html)
- [Compliance](https://www.workday.com/en-us/why-workday/trust/compliance.html)
- [Terms of service](https://www.workday.com/en-us/legal/site-terms.html)
- [Privacy policy](https://www.workday.com/en-us/privacy.html)
- [GitHub](https://github.com/Workday)
- [Status](https://status.workday.com)

## API Evangelist rating

**Kin Score 62.3** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 48.8 |
| Contract governance | 45.5 |
| Operational transparency | 68.4 |
| Developer ergonomics | 72.0 |
| Access clarity | 50.0 |

**Agent readiness 33.4** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | — |

**Regulatory alignment 39.2** — Employment & Payroll

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/workday-business-processes/](https://apis.io/providers/workday-business-processes/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Workday Business Processes: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/workday-business-processes/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
