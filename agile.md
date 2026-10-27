---
layout: default
title: Agile Portfolio
permalink: /agile/
---

# 🧩 Agile Portfolio: WashTrack

[← Back to my portfolio](../)

**Project:** WashTrack, a laundry booking and fault-reporting system for students at New Market Junction, Woodstock, Cape Town.
**Live app:** [WashTrack](https://washtrack-frontend.onrender.com) · **Code:** [GitHub repository](https://github.com/LukhanyoMweli/WashTrack)
**Trello board:** [WashTrack Logbook](https://trello.com/b/IeYy625a)
**Team:** Oluhle Makhaye · Entle Myezo · Lukhanyo Mweli · [fourth member]
**My role:** [e.g. developer: email verification (OTP), UI redesign, deployment]

* * *

## 1. Agile Team Charter

### Evidence

**Purpose:** Build a system that shows which laundry machines are available, occupied or broken, lets students book with their monthly points, and lets South Point review fault reports.

| Element | Details |
|---|---|
| Team values | [your team's values] |
| Roles | Oluhle: [role] · Entle: [role] · Lukhanyo: [role] · [member]: [role] |
| Communication | [e.g. WhatsApp group, Teams meetings] |
| Meetings | [e.g. stand-ups on ... days, sprint review at the end] |
| Definition of Done | Feature works, tested, merged to `master`, deployed on Render |
| Conflict resolution | [how the team settles disagreements] |

![Agile Team Charter on Trello](images/charter.png)

Related completed cards: *Business case research and interviews*, *Trello board setup*, *Team formation and role assignment*, *Complete Agile Charter*.

### Reflection (STAR)

**Situation**
[Why did the team need a charter?]

**Task**
[What was your part?]

**Action**
[What did you suggest or agree? How did the team decide roles?]

**Result**
[What changed in how the team worked? What did you learn about teamwork?]

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

![User stories on Trello](images/trello.png)

### Reflection (STAR)

**Situation**
[What were user stories and why did the team use them?]

**Task**
[Which stories or tasks were yours?]

**Action**
[How did you turn a feature into tasks? What was hard?]

**Result**
[What did you learn about breaking work down?]

* * *

## 3. Product Backlog

### Evidence

| Priority | Item | Story | Status |
|---|---|---|---|
| Must | Basic Registration (email & password) | S1 | [Done] |
| Must | Login authentication | S1 | [Done] |
| Must | User Model in DB | S1 | [Done] |
| Must | Build booking system | S2 | [Done] |
| Must | Create Booking API | S2 | [Done] |
| Must | Booking model (User, Machine, Time Slot) | S2 | [Done] |
| Must | Prevent Double Bookings | S2 | [Done] |
| Should | Build laundry point balance tracker | S3 | [Done] |
| Should | Display Points Balance | S3 | [Done] |
| Should | Display Booking Status | S4 | [Done] |
| Should | Manual status update (Available, Occupied, Broken) | S4 | [Done] |
| Should | Basic Admin Interface | S5 | [Done] |
| Should | Display List of Reports | S5 | [Done] |
| Could | Booking Confirmation Message | S2 | [status] |
| Could | Basic Notification Logic | S6 | [status] |
| Could | Error Handling | S7 | [status] |
| Should | Email verification with OTP | S8 | Done |

![Product backlog on Trello](images/backlog.png)

### Reflection (STAR)

**Situation**
[What was the backlog for?]

**Task**
[How were you involved in building or ordering it?]

**Action**
[How did you decide Must, Should and Could?]

**Result**
[How did prioritising help? What would you do differently?]

* * *

## 4. Sprint Backlog

### Evidence

**Sprint 1:** [start date] to [end date]
**Sprint goal:** Students can register with a verified email, log in, book a machine, see machine status and points, and the app is deployed live.

| Task | Owner | Status |
|---|---|---|
| Email verification with OTP (backend and verify page) | [name] | Done |
| Redesign login, signup and dashboard pages | [name] | Done |
| Fix booking error (app pointed at the wrong database) | [name] | Done |
| Deploy backend and frontend on Render | [name] | [status] |

![Sprint backlog on Trello](images/sprint.png)

### Reflection (STAR)

**Situation**
[What was the sprint goal?]

**Task**
[Which tasks were yours?]

**Action**
[How did you work through them? Describe one real problem and how you solved it.]

**Result**
[Did the team reach the goal? What did the sprint teach you?]

* * *

## 5. Agile Logbook

### Evidence

| Date | Type | What happened | Blockers | Next step |
|---|---|---|---|---|
| [date] | Sprint planning | [sprint goal and cards chosen] | [none] | [start tasks] |
| 2026-10-03 | Work session | Added email verification (OTP) and pushed it to the `email-otp` branch | Gmail login was rejected, so switched to Brevo's email API | Merge to `master` |
| 2026-10-03 | Work session | Pushed the new look (theme and layout) | [none] | Deploy |
| 2026-10-04 | Work session | Fixed "not enough points" bug: the backend was pointed at the wrong database | Login from the old database was stored in the browser | Deploy to Render |
| 2026-10-04 | Work session | Deployed the backend on Render and set its settings | Missing `MONGO_URI`, wrong Brevo key type | Connect the frontend |
| [date] | Stand-up | [what I did / will do] | [issue] | [next] |
| [date] | Retrospective | Went well: [...] · To improve: [...] | [...] | [...] |

### Reflection (STAR)

**Situation**
[Why did the team keep a logbook?]

**Task**
[What did you record?]

**Action**
[How did you keep it up to date?]

**Result**
[How did it help you track progress and problems?]

* * *

*© 2026 Lukhanyo Mweli | CPUT: Faculty of Informatics and Design*
