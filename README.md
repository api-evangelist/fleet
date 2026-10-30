# Fleet

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

Fleet is an open-source device management platform built on osquery. It provides cross-platform MDM, endpoint telemetry, vulnerability and patch management, software inventory, and GitOps-driven configuration for macOS, Windows, Linux, iOS, and Android fleets. Fleet exposes a versioned REST API (/api/v1/fleet, bearer-token auth), the fleetctl CLI for live queries and config-as-code, and outbound webhook automations. It is developed in the open at github.com/fleetdm/fleet and backed by CRV.

**Areas:** Company · Developer Tools · Device Management · MDM · Endpoint Security · Vulnerability Management · osquery · Open Source · DevOps

## Fleet on APIs.io

Everything profiled for Fleet is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fleet/](https://apis.io/providers/fleet/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Fleet API](https://apis.io/apis/fleet/fleet-fleet-api/) — The Fleet API from Fleet — 2 operation(s) for fleet.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Fleet Webhooks](https://apis.io/asyncapis/fleet/fleet-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [fleet](https://apis.io/servers/fleet/fleet/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Fleet Agentic Access](https://apis.io/agentic-access/fleet/fleet-agentic-access/)

#### Collections (1)

Postman and Open Collection request collections.

- [Premium Fleet API](https://apis.io/collections/fleet/open-fleet-fleet-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Fleet Premium Overlay](https://apis.io/overlays/fleet/fleet-premium-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Fleet Authentication](https://apis.io/security/fleet/fleet-authentication/)
- [Fleet Domain Security](https://apis.io/security/fleet/fleet-domain-security/)
- [Fleet Trust Center](https://apis.io/security/fleet/fleet-trust-center/)
- [Fleet Vulnerability Disclosure](https://apis.io/security/fleet/fleet-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://fleetdm.com/)
- [Documentation](https://fleetdm.com/docs)
- [Getting started](https://fleetdm.com/docs/get-started/anatomy)
- [API reference](https://fleetdm.com/docs/rest-api/rest-api)
- [Pricing](https://fleetdm.com/pricing)
- [Sign up](https://fleetdm.com/register)
- [Support](https://fleetdm.com/support)
- [Blog](https://fleetdm.com/articles)
- [Security](https://github.com/fleetdm/fleet/blob/main/SECURITY.md)
- [Compliance](https://trust.fleetdm.com/)
- [Terms of service](https://fleetdm.com/legal/terms)
- [Privacy policy](https://fleetdm.com/legal/privacy)
- [GitHub](https://github.com/fleetdm)
- [Status](https://status.fleetdm.com)

## API Evangelist rating

**Kin Score 55.2** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 44.9 |
| Contract governance | 18.2 |
| Operational transparency | 52.6 |
| Developer ergonomics | 66.1 |
| Access clarity | 60.5 |

**Agent readiness 26.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fleet/](https://apis.io/providers/fleet/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Fleet: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fleet/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
