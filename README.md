# D2L Brightspace (brightspace)

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
