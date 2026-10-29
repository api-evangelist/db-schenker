# DB Schenker

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

DB Schenker (Schenker AG, headquartered in Essen, Germany) is one of the world's largest freight forwarders and contract logistics providers, moving air, ocean, land and rail freight and running warehousing for shippers across roughly 1,850 locations. As a forwarder it sits in the intermediation layer of the supply chain — between the shipper who owns the cargo and the carriers, terminals and customs authorities who move and clear it — buying capacity it does not own and reselling visibility it did not have to publish. Its API posture is honestly a customer-contract posture, not a public developer posture. Deutsche Bahn sold DB Schenker to DSV A/S, completing 30 April 2025, and as of this profile www.dbschenker.com 301-redirects to dsv.com while the global developer portal at api-portal.dbschenker.com answers HTTP 410 Gone. The one DB Schenker-branded machine-readable API surface still live is the Nordic parcel "Partner services API" at parcelservices-se.dbschenker.com/Apipartner, which publishes four Swagger 2.0 documents openly but returns 401 on every operation without HTTP Basic credentials issued against a signed Swedish transport agreement. Its EDI endpoints are proprietary JSON, not EDIFACT or X12, and no DCSA, IATA ONE Record, GS1 EPCIS or WCO Data Model conformant contract was found on any reachable host.

**Areas:** Logistics · Supply Chain · Germany · Freight Forwarding · Parcel · Track and Trace · Customs · Air Cargo · Ocean Freight · Contract Logistics · EDI · Freight

## DB Schenker on APIs.io

Everything profiled for DB Schenker is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/db-schenker/](https://apis.io/providers/db-schenker/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [DB Schenker Delivery Point API](https://apis.io/apis/db-schenker/db-schenker-deliverypoint-api/) — Responsible for all Web API functions related to Service Points
- [DB Schenker Delivery Point2 API](https://apis.io/apis/db-schenker/db-schenker-deliverypoint2-api/) — Responsible for all Web API functions related to Service Points
- [DB Schenker Delivery Point3 API](https://apis.io/apis/db-schenker/db-schenker-deliverypoint3-api/) — Responsible for all Web API functions related to Service Points
- [DB Schenker Delivery Point4 API](https://apis.io/apis/db-schenker/db-schenker-deliverypoint4-api/) — Responsible for all Web API functions related to Service Points
- [DB Schenker Edi API](https://apis.io/apis/db-schenker/db-schenker-edi-api/) — Responsible for all Web API functions related to EDI (For example: Register, Register Return)
- [DB Schenker Extended Delivery Point API](https://apis.io/apis/db-schenker/db-schenker-extendeddeliverypoint-api/) — Responsible for all Web API functions related to HITTA
- [DB Schenker Print Code API](https://apis.io/apis/db-schenker/db-schenker-printcode-api/) — Responsible for (QR) print codes.
- [DB Schenker Sorting Code API](https://apis.io/apis/db-schenker/db-schenker-sortingcode-api/) — Responsible for all Web API functions related to handling sorting codes in MANET.
- [DB Schenker Track And Trace Advanced2 API](https://apis.io/apis/db-schenker/db-schenker-trackandtraceadvanced2-api/) — Responsible for all Web API functions related to Advanced Track and Trace.
- [DB Schenker Track And Trace Boxes API](https://apis.io/apis/db-schenker/db-schenker-trackandtraceboxes-api/) — Responsible for all Web API functions related to Boxes Track and Trace.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Collections (4)

Postman and Open Collection request collections.

- [Partner services API V1.](https://apis.io/collections/db-schenker/open-db-schenker-partner-services-v1-swagger/)
- [Partner services API V2.](https://apis.io/collections/db-schenker/open-db-schenker-partner-services-v2-swagger/)
- [Partner services API V3.](https://apis.io/collections/db-schenker/open-db-schenker-partner-services-v3-swagger/)
- [Partner services API V4.](https://apis.io/collections/db-schenker/open-db-schenker-partner-services-v4-swagger/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.dbschenker.com/)
- [Documentation](https://parcelservices-se.dbschenker.com/Apipartner/Help)
- [API reference](https://parcelservices-se.dbschenker.com/Apipartner/swagger/ui/index)
- [GitHub](https://github.com/dbschenker)

## API Evangelist rating

**Kin Score 21.5** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 43.3 |
| Contract governance | 0.0 |
| Operational transparency | 2.6 |
| Developer ergonomics | 31.0 |
| Access clarity | 0.0 |

**Agent readiness 15.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 0.0** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/db-schenker/](https://apis.io/providers/db-schenker/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for DB Schenker: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/db-schenker/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
