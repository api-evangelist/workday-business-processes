---
name: Approve or deny a Workday business process step
description: >-
  Find the business process event steps awaiting action, read the one you care about, and approve,
  deny or send it back — using the Workday Business Process REST API v1.
api: openapi/workday-business-processes-business-process-openapi.yml
operations:
  - GET /eventSteps
  - GET /eventSteps/{ID}
  - POST /eventSteps/{ID}/approve
  - POST /eventSteps/{ID}/deny
  - POST /eventSteps/{ID}/sendBack
  - GET /values/sendBack/to/
method: generated
generated: '2026-09-17'
source: openapi/_original/workday-business-processes-business-process-v1-openapi.json
---

# Approve or deny a Workday business process step

Base URL: `https://{tenantHostname}/businessProcess/v1` — the tenant's Workday API Gateway host.

> The published spec declares **no `operationId` on any operation**. Bind by method + path, exactly as
> written below; there are no ids to call by name.

## Before you act

1. Get an OAuth 2.0 token for a registered API client on the target tenant. Authorization Code or
   Client Credentials; the client must be allowlisted on that tenant by a Company Administrator.
2. Authorization is two-layered. A valid token is not enough — the tenant's **business process
   security policy** decides whether your security group may approve, deny or send back. A 403 here
   usually means policy, not a bad token.
3. There is **no idempotency mechanism**. Do not blind-retry a `POST .../approve` after a timeout;
   re-read the step with `GET /eventSteps/{ID}` and check its state first.

## Steps

1. **List the steps awaiting action.**
   `GET /eventSteps?limit=20&offset=0` — filter with `businessProcess`, `status`, `worker`,
   `stepType`, and the date-range pairs (`dueDateOnOrAfter`, `dueDateOnOrBefore`,
   `createdOnOrAfter`, `createdOnOrBefore`).
   The response is `{ total, data[] }`. Page by incrementing `offset`; `limit` defaults to 20 and
   caps at 100. There is no cursor and no `Link` header.

2. **Read the one step you intend to act on.**
   `GET /eventSteps/{ID}` where `{ID}` is the step's Workday ID (a 32-character hex WID).
   Never act from the list alone — confirm the step's current state.

3. **Take the action.** All three are `POST` and all three return **201**:
   - Approve: `POST /eventSteps/{ID}/approve` with `{ "comment": "..." }`
   - Deny: `POST /eventSteps/{ID}/deny` with `{ "comment": "..." }`
   - Send back: first `GET /values/sendBack/to/` to read the **valid send-back targets**, then
     `POST /eventSteps/{ID}/sendBack` naming one of them.

4. **Handle the response.** Errors are `application/json` with an `error` string — **not** RFC 9457.
   Every operation declares 400, 401, 403, 404 and a default. There is no error-code registry to
   look a code up in.

## Reversal

An approval is not un-doable as a step. To reverse the outcome you either **send back** to an earlier
step while the process is in flight, or **rescind the whole event** once it has completed
(`POST /events/{ID}/rescind`). Neither has a stated time limit. See
`conventions/workday-business-processes-conventions.yml` for the full reversibility record.

## Rate limiting

Workday publishes **no** `RateLimit-*` or `Retry-After` headers. A 429 is the only signal, and the
threshold is adaptive to tenant load. Use exponential back-off with jitter, and note that a loop of
invalid requests will itself trigger a 429 guardrail.
