---
name: Create and manage custom Workday business process types
description: >-
  Use the Custom Business Process Config API v1 to create, read, update and delete custom business
  process types and their event task definitions.
api: openapi/workday-business-processes-custom-business-process-config-openapi.yml
operations: [create, get, view, update, delete, createEventTaskDefinition, getEventTaskDefinition, viewEventTaskDefinition, updateEventTaskDefinition, patchEventTaskDefinition, deleteEventTaskDefinition]
method: generated
generated: '2026-09-17'
source: openapi/_original/workday-business-processes-custom-business-process-config-v1-openapi.json
---

# Create and manage custom business process types

Base URL: `https://api.workday.com/customBusinessProcessConfig/v1` — note this is the **api.workday.com**
gateway host, not the tenant host used by `businessProcess/v1`. The two business process services in
this record sit on different bases; do not reuse one base for the other.

Auth: OAuth 2.0, authorization URL `https://auth.api.workday.com/v1/authorize`, scopes `read`
(read custom business process types) and `write` (modify custom business process types). These are the
only two named scopes either contract declares.

Unlike `businessProcess/v1`, **this service does declare `operationId`s** — call them by name.

## Business process types

| Intent | operationId | Call |
|---|---|---|
| List types | `get` | `GET /types` |
| Read one type | `view` | `GET /types/{id}` |
| Create a type | `create` | `POST /types` |
| Replace a type | `update` | `PUT /types/{id}` |
| Delete a type | `delete` | `DELETE /types/{id}` |

## Event task definitions

| Intent | operationId | Call |
|---|---|---|
| List | `getEventTaskDefinition` | `GET /eventTaskDefinitions` |
| Read one | `viewEventTaskDefinition` | `GET /eventTaskDefinitions/{id}` |
| Create | `createEventTaskDefinition` | `POST /eventTaskDefinitions` |
| Replace | `updateEventTaskDefinition` | `PUT /eventTaskDefinitions/{id}` |
| Patch | `patchEventTaskDefinition` | `PATCH /eventTaskDefinitions/{id}` |
| Delete | `deleteEventTaskDefinition` | `DELETE /eventTaskDefinitions/{id}` |

## Rules

- **Delete is a hard delete.** There is no restore endpoint, no soft-delete flag and no stated
  retention window. Read the object with `view` before deleting it, and keep the body if you may need
  to recreate it.
- **No idempotency key.** A retried `POST /types` can create a second type. Create, then list and
  verify, rather than retrying blind.
- `create` and `update` return **200** (not 201) on success, with 400 for validation failures and 404
  on an unknown id.
- Configuring the type is only half the job — a custom business process also needs its **security
  policy** configured in the tenant before events can run against it
  (https://developer.workday.com/doc/wyj1518458687942.md).
