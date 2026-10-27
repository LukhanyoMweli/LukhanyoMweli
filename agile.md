---
title: Agile Portfolio
permalink: /agile/
---

# 🧩 Agile Portfolio: WashTrack

[← Back to my portfolio](https://lukhanyomweli.github.io/LukhanyoMweli/)

**Project:** WashTrack, a laundry booking and fault-reporting system for students at New Market Junction, Woodstock, Cape Town.
**Live app:** [WashTrack](https://washtrack-frontend.onrender.com) · **Code:** [GitHub repository](https://github.com/LukhanyoMweli/WashTrack) · **Trello board:** [WashTrack Logbook](https://trello.com/b/IeYy625a)
**Team:** Oluhle Makhaye · Entle Myezo · Lukhanyo Mweli · MM
**My role:** Developer: email verification (OTP), UI redesign, bug fixing and deployment

> **Note:** The live app runs on a free Render server, so the first page load can take up to a minute while the server wakes up.

---

## 1. Agile Team Charter

### Evidence

**Purpose:** Build a system that shows which laundry machines are available, occupied or broken, lets students book with their monthly points, and lets South Point review fault reports.

| Element | Details |
|---|---|
| Team values | Respect, accountability, open communication, and delivering working software |
| Roles | Oluhle: Developer · Entle: Developer · Lukhanyo: Developer (OTP, UI, deployment) · MM: Developer |
| Communication | WhatsApp group for daily updates; Microsoft Teams for meetings |
| Meetings | Short stand-ups during the sprint and a review at the end of the sprint |
| Definition of Done | Feature works, tested, merged to `master`, deployed on Render |
| Conflict resolution | Discuss openly as a team and decide by agreement; ask the lecturer if we cannot agree |

![Agile Team Charter on Trello](https://lukhanyomweli.github.io/LukhanyoMweli/charter.jpg)

Related completed cards: *Business case research and interviews*, *Trello board setup*, *Team formation and role assignment*, *Complete Agile Charter*.

### Reflection (STAR)

**Situation** Our team of four was starting WashTrack and needed shared rules so that everyone knew what was expected of them before we began building.

**Task** I helped agree on how we would communicate, who would own which work, and what "done" meant for our team.

**Action** We set up the Trello board, assigned roles and completed the Agile Charter together. We agreed on a Definition of Done: a feature must work, be tested, be merged to `master` and be deployed on Render before we call it finished.

**Result** The charter gave us a clear standard for finished work and made it easier to see who was responsible for what. I learned that agreeing on expectations early prevents confusion later in a project.

---

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

![User stories on Trello](https://lukhanyomweli.github.io/LukhanyoMweli/trello.jpg)

### Reflection (STAR)

**Situation** WashTrack had many features, such as booking, points, machine status and fault reports. We needed a way to describe each one from the student's point of view.

**Task** I helped turn the features into user stories (S1 to S8) and link each story to its Trello task cards. My own work was mainly S8 (email verification) and fixes to the booking feature.

**Action** For each story we wrote "As a [user], I want…, so that…" and then split it into smaller cards. For example, S2 (booking) became the booking model, the booking API, preventing double bookings and a confirmation message. The hardest part was keeping each task small enough to finish within the sprint.

**Result** I learned that user stories keep the focus on what the student actually needs, and that small tasks make progress easy to see. S8 was added later, which showed me that stories can change as a project grows.

---

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
| Should | Email verification with OTP | S8 | Built; email sending on the live app is being fixed |
| Could | Booking Confirmation Message | S2 | In backlog |
| Could | Basic Notification Logic | S6 | In backlog |
| Could | Error Handling | S7 | In backlog |

![Product backlog on Trello](https://lukhanyomweli.github.io/LukhanyoMweli/backlog.jpg)

On the Trello board, these items are grouped into larger backlog items (Student Dashboard, Laundry Machine Management, Booking Management, Fault Reporting, Manager Dashboard, and Testing & Quality Assurance). Each larger item has a checklist of the detailed tasks listed above, and the checklist counts on the board show how far each one has progressed.

### Reflection (STAR)

**Situation** The product backlog held everything WashTrack might need, so we had to decide what to build first.

**Task** I helped order the backlog items and checked that each one linked back to a user story.

**Action** We used Must, Should and Could. Registration, login and booking were Must, because nothing else works without them. Points and machine status were Should, and notifications and error handling were Could. Later we added email verification (OTP) as a Should item.

**Result** Prioritising kept us focused on a working core first. Next time I would also estimate the effort of each item, so the order reflects both value and difficulty.

---

## 4. Sprint Backlog

### Evidence

**Sprint 4: Testing, Deployment and Documentation** (the sprint my tasks belong to): 1 October 2026 to 6 October 2026
**Sprint goal:** Students can register with a verified email, log in, book a machine, see machine status and points, and the app is deployed live.

| Task | Owner | Status |
|---|---|---|
| Email verification with OTP (backend and verify page) | Lukhanyo | Built; email sending on the live app is being fixed |
| Redesign login, signup and dashboard pages | Lukhanyo | Done |
| Fix booking error (app pointed at the wrong database) | Lukhanyo | Done |
| Deploy backend and frontend on Render | Lukhanyo | Done |

![Sprint backlog on Trello](https://lukhanyomweli.github.io/LukhanyoMweli/sprint.jpg)

The Trello Sprint Backlog column also holds the earlier sprint cards (Sprint 1: Research, Planning and Project Setup; Sprint 2: Authentication and Student Functionality; Sprint 3: Fault Reporting and Manager Functionality). Each card has a checklist that shows progress.

### Reflection (STAR)

**Situation** Our sprint goal was for students to register with a verified email, log in, book a machine, see status and points, and have the app running live.

**Task** I took on email verification with OTP, the redesign of the login, signup and dashboard pages, the booking bug fix and the deployment on Render.

**Action** Gmail rejected my login when sending OTP emails, so I switched to Brevo's email API. Later, booking failed with a "not enough points" error. I traced it to the backend pointing at the wrong database and corrected it. During deployment the backend failed because `MONGO_URI` was missing and I had used the wrong type of Brevo key, so I fixed both settings. After deployment, signup on the live app showed "cannot send verification email", so I checked the Render logs and the Brevo settings to find the cause.

**Result** The app was deployed and most of the sprint goal was reached, with the Sprint 4 checklist showing 11 of 15 items complete. Email verification still needs fixing on the live version. I learned to read error messages carefully, to check configuration first, and that something working locally can still fail once deployed.

---

## 5. Agile Logbook

### Evidence

| Date | Type | What happened | Blockers | Next step |
|---|---|---|---|---|
| 2026-10-01 | Sprint planning | Set the sprint goal and chose the OTP, redesign, bug fix and deployment tasks | None | Start OTP work |
| 2026-10-03 | Work session | Added email verification (OTP) and pushed it to the `email-otp` branch | Gmail login was rejected, so switched to Brevo's email API | Merge to `master` |
| 2026-10-03 | Work session | Pushed the new look (theme and layout) | None | Deploy |
| 2026-10-04 | Work session | Fixed "not enough points" bug: the backend was pointed at the wrong database | Login from the old database was stored in the browser | Deploy to Render |
| 2026-10-04 | Work session | Deployed the backend on Render and set its settings | Missing `MONGO_URI`, wrong Brevo key type | Connect the frontend |
| 2026-10-05 | Stand-up | Done: backend deployed. Doing: connect the frontend to the backend | Frontend not yet connected | Test the live app |
| 2026-10-06 | Retrospective | Went well: OTP and deployment worked in the end. To improve: check configuration earlier and share blockers sooner | Configuration mistakes cost time | Add more testing before deploying |
| 2026-10-27 | Work session | Tested the live app. The backend responded ("WashTrack API is running"), but signup showed "cannot send verification email". Started checking the Render logs and Brevo settings | Email sending fails on the deployed version | Check the Brevo API key type and sender, then redeploy |

![Agile Logbook on Trello](https://lukhanyomweli.github.io/LukhanyoMweli/logbook.jpg)

### Reflection (STAR)

**Situation** We kept a logbook to record what we did, what blocked us and what came next, so progress and problems were not forgotten.

**Task** I recorded each of my work sessions, including the blockers and the next step.

**Action** After every session I added an entry. For example, I logged the Gmail rejection that led me to Brevo, the wrong database that caused the booking error, the missing `MONGO_URI` on Render, and the email error I found when testing the live app.

**Result** The logbook let me see a pattern: configuration errors caused most of our delays. It also made the retrospective easier, because the problems were already written down. I learned that short, regular notes are more useful than trying to remember everything later.

---

*© 2026 Lukhanyo Mweli | CPUT: Faculty of Informatics and Design*
