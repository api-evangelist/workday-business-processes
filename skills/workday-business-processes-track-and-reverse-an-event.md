---
name: Track a Workday business process event and cancel or rescind it
description: >-
  Follow a business process event through its steps, read its comments and attachments, and reverse it
  — cancel while in progress, rescind once complete.
api: openapi/workday-business-processes-business-process-openapi.yml
operations:
  - GET /events
  - GET /events/{ID}
  - GET /events/{ID}/inProgressSteps
  - GET /events/{ID}/remainingSteps
  - GET /events/{ID}/completedSteps
  - GET /events/{ID}/comments
  - GET /events/{ID}/attachments
  - POST /events/{ID}/cancel
  - POST /events/{ID}/rescind
method: generated
generated: '2026-09-17'
source: openapi/_original/workday-business-processes-business-process-v1-openapi.json
---

# Track a Workday business process event, and reverse it

Base URL: `https://{tenantHostname}/businessProcess/v1`.

A business process **event** is one running instance of a business process definition. You do not
create one here — events are started elsewhere (a Workday UI task, or a `POST` on another service such
as `POST /workers/{ID}/jobChanges` in staffing). This API observes and controls an event that already
exists.

## Steps

1. **Find the event.**
   `GET /events` with the filters that matter: `businessProcess`, `status`, `initiator`,
   `eventTarget`, `worker`, and the date ranges `initiatedOnOrAfter` / `initiatedOnOrBefore` and
   `completedOnOrAfter` / `completedOnOrBefore`. Response is `{ total, data[] }`, `limit` max 100.

2. **Read its state.** `GET /events/{ID}`.

3. **Walk the process.** Three separate collections, not one:
   - `GET /events/{ID}/inProgressSteps`
   - `GET /events/{ID}/remainingSteps`
   - `GET /events/{ID}/completedSteps`

4. **Read the human context.** `GET /events/{ID}/comments` and `GET /events/{ID}/attachments`.
   Attachment categories for the process type come from
   `GET /types/{ID}/attachmentCategories`.

## Reversing the event

- **Cancel — while the event is in progress.** `POST /events/{ID}/cancel` with
  `{ "comment": "..." }`. The docs describe it as "cancel or immediately end" the event. Returns 201.
- **Rescind — after the event has completed.** `POST /events/{ID}/rescind` with
  `{ "comment": "..." }`. Returns 201.

Two things the docs state that you must not assume away:

- For **Extend** business processes, the definition must have **Enable Cancellation** / **Enable
  Rescind** set to `true`, or the call will not be permitted.
- **Rescind on an Extend process marks the event rescinded; it does NOT roll back data.** Workday's
  own guidance is to build a custom orchestration to perform the rollback actions. Do not report a
  rescind to a user as "the change was undone" unless you know the process is Workday-delivered.

Workday publishes **no time-bounded window** for either. The window is state-based: in progress →
cancel; completed → rescind.

## Discovery

`GET /types` lists the business process types in the tenant, `GET /types/{ID}` reads one. Use it to
resolve the `businessProcess` filter value before querying events.
