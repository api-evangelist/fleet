---
name: Manage Fleet teams
description: Create, list, retrieve, and delete teams in Fleet (Premium) via the REST API, using bearer-token auth and Fleet's pagination and error conventions.
api: openapi/fleet-premium-openapi.json
operations:
  - GET /api/v1/fleet/teams
  - POST /api/v1/fleet/teams
  - GET /api/v1/fleet/teams/{id}
  - DELETE /api/v1/fleet/teams/{id}
---

# Manage Fleet teams

Fleet Teams (a Fleet Premium feature) group hosts so you can apply distinct
configuration, policies, and enroll secrets per group.

## Authentication
All requests require a bearer token in the `Authorization` header:

```
Authorization: Bearer <token>
```

For automation, create an API-only user (`fleetctl user create --api-only`) — its
token does not expire. SSO/MFA users must copy a token from the Fleet UI
("My account" > Get API token). See `authentication/fleet-authentication.yml`.

## Steps

1. **List existing teams** — `GET /api/v1/fleet/teams`. Supports pagination
   (`page`, `per_page`) and ordering (`order_key`, `order_direction`), plus a
   `query` keyword search over the team name. The response is `{ "teams": [ ... ] }`.

2. **Create a team** — `POST /api/v1/fleet/teams` with a JSON body
   `{ "name": "<required>", "description": "...", "agent_options": "..." }`.
   `name` is required. The created `Team` object is returned, including its `id`
   and any enroll `secrets`.

3. **Get a team** — `GET /api/v1/fleet/teams/{id}` to read a single team by its
   integer `id`.

4. **Delete a team** — `DELETE /api/v1/fleet/teams/{id}`. This is destructive;
   confirm the `id` first with step 1 or 3.

## Conventions & error handling
- **Pagination**: `page` / `per_page` (up to 10,000 records); order with
  `order_key` + `order_direction` (`asc`/`desc`).
- **Errors** return a JSON envelope `{ message, errors: [{name, reason}], uuid }`.
  Common statuses: `401` invalid/missing token, `403` RBAC-forbidden, `404` not
  found, `422` validation error (check `errors[]`), `429` rate limited (respect
  the `retry-after` header, in seconds). Share the `uuid` with support for `500`s.
  See `errors/fleet-problem-types.yml`.
- **Idempotency**: Fleet has no Idempotency-Key header. For convergent, safe-retry
  management, prefer the GitOps flow (`fleetctl gitops`) over ad-hoc mutations.
