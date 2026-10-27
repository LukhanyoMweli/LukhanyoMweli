---
layout: default
title: Agile Portfolio
permalink: /agile/
---

# 🧩 Agile Portfolio: WashTrack

[← Back to my portfolio](../)

- **Project:** WashTrack, a laundry booking and fault-reporting system for students at New Market Junction, Woodstock, Cape Town
- **Live app:** [WashTrack](https://washtrack-frontend.onrender.com)
- **Code:** [GitHub repository](https://github.com/LukhanyoMweli/WashTrack)
- **Trello board:** [WashTrack Logbook](https://trello.com/b/IeYy625a)
- **Team:** Oluhle Makhaye · Lukhanyo Mweli 
- **My role:** Developer (email verification, UI redesign, deployment)

* * *

## 1. Agile Team Charter

### Evidence

**Purpose:** To build a system that shows which laundry machines are available, occupied or broken, lets students book with their monthly laundry points, and lets South Point review fault reports.

| Element | Details |
|---|---|
| Team values | CONFIRM: copy from your charter card |
| Roles | CONFIRM: each member and their role |
| Communication | CONFIRM: e.g. WhatsApp group, Microsoft Teams |
| Meetings | CONFIRM: how often the team met |
| Definition of Done | CONFIRM: copy from your charter |
| Conflict resolution | CONFIRM: copy from your charter |

![Agile Team Charter on Trello](../images/charter.png)

Related completed Trello cards: *Business case research and interviews*, *Trello board setup*, *Team formation and role assignment* and *Complete Agile Charter*.

### Reflection (STAR)

<!-- Real things you can use: a four-person team agreeing roles; the charter card was assigned to all members; the business case came from resident interviews. Write it in your own words. -->

**Situation**
WRITE:

**Task**
WRITE:

**Action**
WRITE:

**Result**
WRITE:

* * *

## 2. User Stories and Tasks

### Evidence

| ID | User story | Tasks (Trello cards) |
|---|---|---|
| S1 | As a student, I want to register and log in, so my laundry points belong to me. | Basic Registration · Login authentication · User Model in DB |
| S2 | As a student, I want to book a free machine, so I can reserve it. | Build booking system · Create Booking API · Booking model (User, Machine, Time Slot) · Prevent Double Bookings · Booking Confirmation Message |
| S3 | As a student, I want to see my points balance, so I can plan my washes. | Build laundry point balance tracker · Display Points Balance |
| S4 | As a student, I want to see which machines are available, occupied or broken, so I don't waste a trip. | Display Booking Status · Manual status update |
| S5 | As an admin, I want to see reported faults and update machines, so repairs happen and students are refunded. | Basic Admin Interface · Display List of Reports |
| S6 | As a student, I want to be notified about my booking, so I don't miss my turn. | Basic Notification Logic |
| S7 | As a user, I want clear errors when something fails, so I know what to do. | Error Handling |
| S8 | As a new user, I want to verify my email with a code, so only real emails can register. | Email verification with OTP (added later) |

![User stories on Trello](../images/trello.png)

### Reflection (STAR)

<!-- Real things you can use: how a card like "Build booking system" became a student outcome; grouping 16 technical cards into stories; adding S8 later when email verification was needed. -->

**Situation**
WRITE:

**Task**
WRITE:

**Action**
WRITE:

**Result**
WRITE:

* * *

## 3. Product Backlog

### Evidence

| Priority | Item | Story | Status |
|---|---|---|---|
| Must | Basic Registration (email & password) | S1 | Done |
| Must | Login authentication | S1 | Done |
| Must | User Model in DB | S1 | Done |
| Must | Build booking system | S2 | Done |
| Must | Create Booking API | S2 | Done |
| Must | Booking model (User, Machine, Time Slot) | S2 | Done |
| Must | Prevent Double Bookings | S2 | Done |
| Should | Build laundry point balance tracker | S3 | Done |
| Should | Display Points Balance | S3 | Done |
| Should | Display Booking Status | S4 | Done |
| Should | Manual status update (Available, Occupied, Broken) | S4 | Done |
| Should | Basic Admin Interface | S5 | Done |
| Should | Display List of Reports | S5 | Done |
| Could | Booking Confirmation Message | S2 | CONFIRM: status |
| Could | Basic Notification Logic | S6 | CONFIRM: status |
| Could | Error Handling | S7 | CONFIRM: status |
| Should | Email verification with OTP | S8 | Done |

![Product backlog on Trello](../images/backlog.png)

### Reflection (STAR)

<!-- Real things you can use: how Must/Should/Could were chosen; which cards were left unbuilt and why; what you would prioritise differently. -->

**Situation**
WRITE:

**Task**
WRITE:

**Action**
WRITE:

**Result**
WRITE:

* * *

## 4. Sprint Backlog

### Evidence

- **Sprint:** CONFIRM: start date to end date
- **Sprint goal:** Students can register with a verified email, log in, book a machine, see machine status and points, and the app is deployed live.

| Task | Owner | Status |
|---|---|---|
| Email verification with OTP (backend and verify page) | CONFIRM: name | Done |
| Redesign login, signup and dashboard pages | CONFIRM: name | Done |
| Fix booking error (app was pointed at the wrong database) | CONFIRM: name | Done |
| Deploy the backend on Render | CONFIRM: name | Done |
| Connect the live frontend to the backend | CONFIRM: name | CONFIRM: status |

![Sprint backlog on Trello](../images/sprint.png)

### Reflection (STAR)

<!-- Real things you can use: the booking bug (a login saved from a different database made the app report "not enough points"); Brevo's SMTP key vs API key and its IP blocking; Render needing its own environment settings; keeping secrets out of GitHub. -->

**Situation**
WRITE:

**Task**
WRITE:

**Action**
WRITE:

**Result**
WRITE:

* * *

## 5. Agile Logbook

### Evidence

| Date | Type | What happened | Blockers | Next step |
|---|---|---|---|---|
| CONFIRM: date | Sprint planning | CONFIRM: sprint goal and cards chosen | CONFIRM | CONFIRM |
| 2026-10-03 | Work session | Built email verification (OTP) and pushed it to the `email-otp` branch | Gmail login was rejected, so switched to Brevo's email API | Merge to `master` |
| 2026-10-04 | Work session | Fixed the "not enough points" booking error: the backend had been pointed at the wrong database | An old login saved in the browser | Deploy to Render |
| 2026-10-04 | Work session | Deployed the backend on Render and added its environment settings | Missing database setting; SMTP key used instead of API key | Connect the frontend |
| CONFIRM: date | Stand-up | CONFIRM: what the team did and planned | CONFIRM | CONFIRM |
| CONFIRM: date | Retrospective | Went well: CONFIRM · To improve: CONFIRM | CONFIRM | CONFIRM |

### Reflection (STAR)

<!-- Real things you can use: how dated entries helped you trace problems; how git history and Trello backed up the log; what you would record more often. -->

**Situation**
WRITE:

**Task**
WRITE:

**Action**
WRITE:

**Result**
WRITE:

* * *

*© 2026 Lukhanyo Mweli | CPUT: Faculty of Informatics and Design*
