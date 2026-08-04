# D2L Brightspace (brightspace)

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

D2L Brightspace is an enterprise learning management system (LMS) used by higher education, K-12, and corporate organizations. Its public REST API is the **Valence Learning Framework API**, served from each institution's own Brightspace host under `https://{host}/d2l/api/`. Routes are split into two product components - **lp** (Learning Platform: users, roles, enrollments, org units, Data Hub) and **le** (Learning Environment: content, grades, assignments/dropbox, quizzes, discussions, calendar, news, learning outcomes) - and each component is independently versioned (for example `lp/1.53` or `le/1.92`; confirm supported versions via `GET /d2l/api/versions/`). Requests are authenticated with OAuth 2 bearer tokens issued by the D2L auth service using the authorization code grant; the older ID-Key (app-id/user-id signed URL) scheme is deprecated. "D2L" is the vendor, "Brightspace" the product, and "Valence" the historical name of the API framework.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/apis.yml)

## Tags

- LMS
- Learning Management System
- EdTech
- Education
- Valence
- D2L
- Brightspace

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Brightspace Users API

Manage user accounts on the Learning Platform - retrieve the current caller (whoami), list and search users, create, update, and delete users, manage names, activation, pronouns, and passwords, and read the role catalog.

- **Human URL:** [https://docs.valence.desire2learn.com/res/user.html](https://docs.valence.desire2learn.com/res/user.html)
- **Base URL:** `https://{host}/d2l/api/lp`

### Brightspace Enrollments API

Enroll and unenroll users in org units, list users enrolled in a course or department, list a user's org units, read the caller's own enrollments, and run batch enrollment operations.

- **Human URL:** [https://docs.valence.desire2learn.com/res/enroll.html](https://docs.valence.desire2learn.com/res/enroll.html)
- **Base URL:** `https://{host}/d2l/api/lp`

### Brightspace Org Units API

Read and manage the organization structure - org units and their relationships, org unit types, course offerings, departments and semesters, the recycle bin, and organization info.

- **Human URL:** [https://docs.valence.desire2learn.com/res/orgunit.html](https://docs.valence.desire2learn.com/res/orgunit.html)
- **Base URL:** `https://{host}/d2l/api/lp`

### Brightspace Content API

Build and read course content - the root table of contents, modules and their structure, and topics and topic files within a course offering.

- **Human URL:** [https://docs.valence.desire2learn.com/res/content.html](https://docs.valence.desire2learn.com/res/content.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Grades API

Read and write the course gradebook - grade objects, per-user grade values (including my grades), final calculated grades, grade categories, grade schemes, and exemptions.

- **Human URL:** [https://docs.valence.desire2learn.com/res/grade.html](https://docs.valence.desire2learn.com/res/grade.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Assignments (Dropbox) API

Manage assignment (Dropbox) folders and categories, read and create learner submissions, download submitted files, and post instructor feedback and attachments.

- **Human URL:** [https://docs.valence.desire2learn.com/res/dropbox.html](https://docs.valence.desire2learn.com/res/dropbox.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Quizzes API

Create and read quizzes, list attempts and questions, manage quiz categories, and configure per-learner special access.

- **Human URL:** [https://docs.valence.desire2learn.com/res/quiz.html](https://docs.valence.desire2learn.com/res/quiz.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Discussions API

Manage discussion forums, topics, and posts, including replies, ratings, flags, read status, approval, and attachments.

- **Human URL:** [https://docs.valence.desire2learn.com/res/discuss.html](https://docs.valence.desire2learn.com/res/discuss.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Calendar API

Create, read, update, and delete course calendar events, list events and occurrences, and manage event presenters.

- **Human URL:** [https://docs.valence.desire2learn.com/res/calendar.html](https://docs.valence.desire2learn.com/res/calendar.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace News (Announcements) API

Create, read, update, publish, dismiss, and delete news (announcement) items, manage attachments, and configure cross-org-unit sharing.

- **Human URL:** [https://docs.valence.desire2learn.com/res/news.html](https://docs.valence.desire2learn.com/res/news.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Learning Outcomes API

Manage learning outcome sets and outcomes at the organization and org unit level, bulk import/export outcomes, and read and create outcome alignments against course activities.

- **Human URL:** [https://docs.valence.desire2learn.com/res/outcomes.html](https://docs.valence.desire2learn.com/res/outcomes.html)
- **Base URL:** `https://{host}/d2l/api/le`

### Brightspace Data Hub API

Discover and export bulk institutional data through the Data Hub and Data Export Framework - list data sets, create and monitor export jobs, download CSV/ZIP results, and enumerate Brightspace Data Sets extracts.

- **Human URL:** [https://docs.valence.desire2learn.com/res/dataExport.html](https://docs.valence.desire2learn.com/res/dataExport.html)
- **Base URL:** `https://{host}/d2l/api/lp`

## Authentication

The Valence API uses OAuth 2 (authorization code grant). Register an application in Brightspace to obtain a client ID and secret, direct a user through the D2L auth service to obtain an authorization code, and exchange it at the token endpoint (`https://auth.brightspace.com/core/connect/token`) for a short-lived access token plus refresh token. Send `Authorization: Bearer <access_token>` on every request. Scopes take the form `group:resource:action` (for example `users:userdata:read`). The legacy ID-Key authentication scheme is deprecated.

## Common Properties

- [GitHub Organization](https://github.com/Brightspace)
- [LinkedIn](https://www.linkedin.com/company/d2l)
- [Website](https://www.d2l.com)
- [Documentation](https://docs.valence.desire2learn.com)
- [Plans](plans/brightspace-plans-pricing.yml)
- [Rate Limits](rate-limits/brightspace-rate-limits.yml)
- [Fin Ops](finops/brightspace-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
