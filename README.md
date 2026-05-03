# Workday Business Processes (workday-business-processes)
APIs for managing and executing business processes within Workday, including initiating, monitoring, and completing various workflow processes.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Approvals, Business Processes, Enterprise, Finance, HCM, Workflows, Workday

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-03

## APIs

### Workday Business Process API
RESTful API for initiating, managing, and monitoring business processes in Workday including approvals, onboarding workflows, process definitions, inbox items, and process step management. Enables organizations to programmatically trigger Workday business processes and integrate workflow automation with external systems.

**Human URL:** [https://www.workday.com/en-us/products/financial-management/business-process.html](https://www.workday.com/en-us/products/financial-management/business-process.html)


#### Tags:

 - Approvals, Business Processes, Finance, HCM, Workflows

#### Properties

- [Documentation](https://community.workday.com/sites/default/files/file-hosting/productionapi/index.html)
- [OpenAPI](https://community.workday.com/sites/default/files/file-hosting/productionapi/Business_Process_Service/v41.1/Business_Process_Service.yaml)
- [Authentication](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/wws-authentication.html)
- [SDKs](https://github.com/Workday)
- [Rate Limits](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/wws-rate-limits.html)
- [Webhooks](https://doc.workday.com/admin-guide/en-us/workday-integrations/integration-concepts/workday-webhooks.html)
- [Changelog](https://community.workday.com/api-release-notes)
- [Status](https://status.workday.com)
- [Support](https://community.workday.com)
- [OpenAPI](openapi/workday-business-processes-openapi.yml)
- [JSONSchema](json-schema/workday-business-processes-business-process-definition-schema.json)
- [JSONSchema](json-schema/workday-business-processes-process-instance-schema.json)
- [JSONSchema](json-schema/workday-business-processes-process-step-schema.json)
- [JSONSchema](json-schema/workday-business-processes-inbox-item-schema.json)
- [JSONSchema](json-schema/workday-business-processes-approval-request-schema.json)
- [NaftikoCapability - Workflow Management](capabilities/workflow-management.yaml)
- [NaftikoCapability - Business Processes (Shared)](capabilities/shared/business-processes.yaml)

## Common Properties

- [Portal](https://community.workday.com)
- [Getting Started](https://doc.workday.com/admin-guide/en-us/workday-web-services/wws-overview/getting-started-with-workday-web-services.html)
- [API Standards](https://doc.workday.com/admin-guide/en-us/workday-rest-api/workday-rest-api-overview.html)
- [Privacy Policy](https://www.workday.com/en-us/privacy.html)
- [Terms of Service](https://www.workday.com/en-us/terms-of-service.html)
- [Security](https://www.workday.com/en-us/why-workday/our-technology/security.html)
- [JSON-LD](json-ld/workday-business-processes-context.jsonld)
- [SpectralRules](rules/workday-business-processes-spectral-rules.yml)
- [NaftikoCapability - Workflow Management](capabilities/workflow-management.yaml)
- [NaftikoCapability - Business Processes (Shared)](capabilities/shared/business-processes.yaml)
- [Vocabulary](vocabulary/workday-business-processes-vocabulary.yml)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Workday Business Process API](openapi/workday-business-processes-openapi.yml)

### JSON Schema

- [Business Process Definition](json-schema/workday-business-processes-business-process-definition-schema.json)
- [Process Instance](json-schema/workday-business-processes-process-instance-schema.json)
- [Initiate Process Request](json-schema/workday-business-processes-initiate-process-request-schema.json)
- [Process Step](json-schema/workday-business-processes-process-step-schema.json)
- [Inbox Item](json-schema/workday-business-processes-inbox-item-schema.json)
- [Approval Request](json-schema/workday-business-processes-approval-request-schema.json)
- [Denial Request](json-schema/workday-business-processes-denial-request-schema.json)

### JSON Structure

- [Business Process Definition](json-structure/workday-business-processes-business-process-definition-structure.json)
- [Process Instance](json-structure/workday-business-processes-process-instance-structure.json)
- [Initiate Process Request](json-structure/workday-business-processes-initiate-process-request-structure.json)
- [Process Step](json-structure/workday-business-processes-process-step-structure.json)
- [Inbox Item](json-structure/workday-business-processes-inbox-item-structure.json)
- [Approval Request](json-structure/workday-business-processes-approval-request-structure.json)
- [Denial Request](json-structure/workday-business-processes-denial-request-structure.json)

### JSON-LD

- [Workday Business Processes Context](json-ld/workday-business-processes-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Business Processes](capabilities/shared/business-processes.yaml) — 9 operations for process definition, instance, inbox item, and approval management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Workflow Management](capabilities/workflow-management.yaml) | Workday Business Process API | 10 | Manager, HR Business Partner, System Administrator |

## Vocabulary

- [Workday Business Processes Vocabulary](vocabulary/workday-business-processes-vocabulary.yml) — Unified taxonomy mapping 5 resources, 6 actions, 1 workflow, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Workday Business Processes Spectral Rules](rules/workday-business-processes-spectral-rules.yml) — 40 rules across 14 categories enforcing Workday Business Process API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
