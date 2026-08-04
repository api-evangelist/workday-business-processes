# Workday Business Processes (workday-business-processes)

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

APIs for managing and executing business processes within Workday, including initiating, monitoring, and completing various workflow processes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/apis.yml)

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-19

## APIs

### Workday Business Process API

API for initiating, managing, and monitoring business processes in Workday, including approvals, onboarding, and other workflow operations.

- **Human URL:** [https://www.workday.com/en-us/products/financial-management/business-process.html](https://www.workday.com/en-us/products/financial-management/business-process.html)
- **Base URL:** `https://wd2-impl-services1.workday.com/ccx/service`

#### Tags

- Approvals
- Business Processes
- Finance
- HCM
- Workflows

#### Properties

- [Documentation](https://community.workday.com/sites/default/files/file-hosting/productionapi/index.html)
- [OpenAPI](https://community.workday.com/sites/default/files/file-hosting/productionapi/Business_Process_Service/v41.1/Business_Process_Service.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Authentication](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/wws-authentication.html)
- [S D Ks](https://github.com/Workday)
- [Rate Limits](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/wws-rate-limits.html)
- [Webhooks](https://doc.workday.com/admin-guide/en-us/workday-integrations/integration-concepts/workday-webhooks.html)
- [Changelog](https://community.workday.com/api-release-notes)
- [Status Page](https://status.workday.com)
- [Support](https://community.workday.com)
- [OpenAPI](openapi/workday-business-processes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/workday-business-processes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/workday-business-processes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/workday-business-processes-business-process-definition-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-process-instance-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-initiate-process-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-process-step-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-inbox-item-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-approval-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/workday-business-processes-denial-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/workday-business-processes-business-process-definition-structure.json)
- [JSON Structure](json-structure/workday-business-processes-process-instance-structure.json)
- [JSON Structure](json-structure/workday-business-processes-initiate-process-request-structure.json)
- [JSON Structure](json-structure/workday-business-processes-process-step-structure.json)
- [JSON Structure](json-structure/workday-business-processes-inbox-item-structure.json)
- [JSON Structure](json-structure/workday-business-processes-approval-request-structure.json)
- [JSON Structure](json-structure/workday-business-processes-denial-request-structure.json)
- [JSON-LD](json-ld/workday-business-processes-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/workday-business-processes-spectral-rules.yml)
- [Naftiko Capability -  Workflow  Management](capabilities/workflow-management.yaml)
- [Naftiko Capability -  Business  Processes ( Shared)](capabilities/shared/business-processes.yaml)
- [Vocabulary](vocabulary/workday-business-processes-vocabulary.yml)

## Common Properties

- [Portal](https://community.workday.com)
- [Getting Started](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/getting-started-with-workday-web-services.html)
- [A P I  Standards](https://doc.workday.com/admin-guide/en-us/workday-rest-api/workday-rest-api-overview.html)
- [Privacy Policy](https://www.workday.com/en-us/privacy.html)
- [Terms of Service](https://www.workday.com/en-us/terms-of-service.html)
- [Security](https://www.workday.com/en-us/why-workday/our-technology/security.html)
- [JSON-LD](json-ld/workday-business-processes-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/workday-business-processes-spectral-rules.yml)
- [Naftiko Capability -  Workflow  Management](capabilities/workflow-management.yaml)
- [Naftiko Capability -  Business  Processes ( Shared)](capabilities/shared/business-processes.yaml)
- [Vocabulary](vocabulary/workday-business-processes-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
