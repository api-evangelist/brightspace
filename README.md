# D2L Brightspace

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

D2L Brightspace is an enterprise learning management system (LMS) used by higher education, K-12, and corporate organizations. Its public REST API is the Valence Learning Framework API, exposed under https://{host}/d2l/api/ and split into two product components - "lp" (Learning Platform - users, roles, enrollments, org units, data hub) and "le" (Learning Environment - content, grades, assignments/dropbox, quizzes, discussions, calendar, news, learning outcomes). Routes are versioned per component (for example lp 1.x and le 1.x) and authenticated with OAuth 2 bearer tokens issued by the D2L auth service; the older ID-Key (app-id/user-id) scheme is deprecated. D2L is the vendor; Valence is the historical name of the API framework.

**Areas:** LMS · EdTech · Education · Valence · D2L · Brightspace · Canada

## D2L Brightspace on APIs.io

Everything profiled for D2L Brightspace is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/brightspace/](https://apis.io/providers/brightspace/)** — or go straight to one of the APIs or properties below.

### APIs (16)

- [D2L Brightspace Assignments API](https://apis.io/apis/brightspace/brightspace-assignments-api/) — Assignment (Dropbox) folders, submissions, and feedback.
- [D2L Brightspace Calendar API](https://apis.io/apis/brightspace/brightspace-calendar-api/) — Course calendar events.
- [D2L Brightspace Content API](https://apis.io/apis/brightspace/brightspace-content-api/) — Course content - modules and topics.
- [D2L Brightspace Data Hub API](https://apis.io/apis/brightspace/brightspace-data-hub-api/) — The Data Hub API provides access to bulk data export functionality, enabling institutions to extract large datasets of users, enrollments, grades, activity,…
- [D2L Brightspace Discussions API](https://apis.io/apis/brightspace/brightspace-discussions-api/) — Discussion forums, topics, and posts.
- [D2L Brightspace Enrollments API](https://apis.io/apis/brightspace/brightspace-enrollments-api/) — Membership of users in org units.
- [D2L Brightspace Grades API](https://apis.io/apis/brightspace/brightspace-grades-api/) — Course gradebook - grade objects, values, categories, and schemes.
- [D2L Brightspace Learning Outcomes API](https://apis.io/apis/brightspace/brightspace-learning-outcomes-api/) — Learning outcome sets, outcomes, and alignments.
- [D2L Brightspace News API](https://apis.io/apis/brightspace/brightspace-news-api/) — News (announcement) items.
- [D2L Brightspace Org Units API](https://apis.io/apis/brightspace/brightspace-org-units-api/) — Organization structure, course offerings, departments, and semesters.
- [D2L Brightspace Quizzes API](https://apis.io/apis/brightspace/brightspace-quizzes-api/) — Quizzes, attempts, questions, and special access.
- [D2L Brightspace Users API](https://apis.io/apis/brightspace/brightspace-users-api/) — User accounts and roles on the Learning Platform.
- [D2L Brightspace Versions API](https://apis.io/apis/brightspace/brightspace-versions-api/) — Product component version discovery.
- [Brightspace Learning Environment (LE) API](https://apis.io/apis/brightspace/brightspace-le-api/) — The Learning Environment API provides access to course content, dropbox folders, grade objects, grade values, quizzes, surveys, discussions, forums,…
- [Brightspace ePortfolio API](https://apis.io/apis/brightspace/brightspace-eportfolio-api/) — The ePortfolio API enables management of ePortfolio objects including artifacts, reflections, collections, activities, presentations, and objectives.…
- [Brightspace IPSIS (SIS Integration) API](https://apis.io/apis/brightspace/brightspace-ipsis-api/) — The IPSIS API provides a standardized interface for Student Information System (SIS) integration with Brightspace, enabling automated provisioning and…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [D2L Brightspace GraphQL Schema](https://apis.io/graphqls/brightspace/d2l-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Brightspace Agentic Access](https://apis.io/agentic-access/brightspace/brightspace-agentic-access/)

#### Collections (14)

Postman and Open Collection request collections.

- [D2L Brightspace Valence API](https://apis.io/collections/brightspace/open-brightspace/)
- [D2L Brightspace Valence Learning Framework Assignments API](https://apis.io/collections/brightspace/open-brightspace-assignments-api/)
- [D2L Brightspace Valence Learning Framework Assignments Calendar API](https://apis.io/collections/brightspace/open-brightspace-calendar-api/)
- [D2L Brightspace Valence Learning Framework Assignments Content API](https://apis.io/collections/brightspace/open-brightspace-content-api/)
- [D2L Brightspace Valence Learning Framework Assignments Data Hub API](https://apis.io/collections/brightspace/open-brightspace-data-hub-api/)
- [D2L Brightspace Valence Learning Framework Assignments Discussions API](https://apis.io/collections/brightspace/open-brightspace-discussions-api/)
- [D2L Brightspace Valence Learning Framework Assignments Enrollments API](https://apis.io/collections/brightspace/open-brightspace-enrollments-api/)
- [D2L Brightspace Valence Learning Framework Assignments Grades API](https://apis.io/collections/brightspace/open-brightspace-grades-api/)
- [D2L Brightspace Valence Learning Framework Assignments Learning Outcomes API](https://apis.io/collections/brightspace/open-brightspace-learning-outcomes-api/)
- [D2L Brightspace Valence Learning Framework Assignments News API](https://apis.io/collections/brightspace/open-brightspace-news-api/)
- [D2L Brightspace Valence Learning Framework Assignments Org Units API](https://apis.io/collections/brightspace/open-brightspace-org-units-api/)
- [D2L Brightspace Valence Learning Framework Assignments Quizzes API](https://apis.io/collections/brightspace/open-brightspace-quizzes-api/)
- [D2L Brightspace Valence Learning Framework Assignments Users API](https://apis.io/collections/brightspace/open-brightspace-users-api/)
- [D2L Brightspace Valence Learning Framework Assignments Versions API](https://apis.io/collections/brightspace/open-brightspace-versions-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Brightspace Authentication](https://apis.io/security/brightspace/brightspace-authentication/)
- [Brightspace Domain Security](https://apis.io/security/brightspace/brightspace-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Brightspace Scopes](https://apis.io/scopes/brightspace/brightspace-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Brightspace Plans Pricing](https://apis.io/plans/brightspace/brightspace-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Brightspace Rate Limits](https://apis.io/rate-limits/brightspace/brightspace-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Brightspace Finops](https://apis.io/finops/brightspace/brightspace-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.d2l.com)
- [Documentation](https://docs.valence.desire2learn.com)
- [Blog](https://www.d2l.com/blog/all/)
- [GitHub](https://github.com/Brightspace)

## API Evangelist rating

**Kin Score 27.6** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 47.6 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 32.1 |
| Access clarity | 7.9 |

**Agent readiness 22.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
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
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 21.6** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/brightspace/](https://apis.io/providers/brightspace/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for D2L Brightspace: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/brightspace/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
