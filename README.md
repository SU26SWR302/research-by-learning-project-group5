# JAEN — SWD392 Group 5 · Sum26

**JAEN** (Just Another English Network) is a smart online language learning platform (Smart Language Learning Platform) operating on an open marketplace model that connects learners with certified content creators. Beyond static video lectures, JAEN integrates diverse interactive modules (Flashcards, Quizzes, Reading, Listening), AI-powered automated assessment for Speaking and Writing skills, a personalized progress tracking system, and a personal vocabulary dictionary.

---

## Group 5 — Team Members

| Name | Role |
|---|---|
| Lê Đức Sự | — |
| Lê Viết Mạnh | — |
| Phạm Thị Vân Thanh | — |
| Hoàng Thủy Nguyên | — |
| Huỳnh Tấn Vinh | — |

---

## Project Links

| Resource | Link |
|---|---|
| Jira Board | https://vaanthanh2005.atlassian.net/jira/software/projects/SCRUM/summary |
| Overleaf (Edit) | https://www.overleaf.com/4497129322htpwwdtqcgfx#3fb35e |
| Overleaf (View) | https://www.overleaf.com/read/vtkgtzwpbhgp#2c21c0 |
| Zotero Library | https://www.zotero.org/groups/6586964/jaen-swd392-group5/library |
| RDS Document | https://docs.google.com/document/d/1TkzdZRSMXzru4KWArm73BzWpnXa4SvUaAgt468msgJk/edit?usp=sharing |

---

## System Actors

The JAEN system defines four primary actor roles:

- **Learner** — browses and accesses learning materials, completes assessments, submits Speaking/Writing for AI evaluation, manages personal vocabulary and learning progress.
- **Content Manager (Creator)** — creates and publishes courses, uploads interactive modules, manages media assets, and uses AI-assisted content generation tools.
- **Administrator** — manages user accounts and role assignments, configures system plugins, monitors analytics and audit logs, moderates reported content.
- **AI Engine** — processes Speaking/Writing submissions, generates draft learning content on request, and returns structured evaluation results asynchronously.

---

## Requirements-Based Learning (RBL) Focus

**Research topic:** *Automated AI Assessment System for Language Proficiency (Speaking & Writing)*

**Rationale:** Traditional evaluation of Speaking and Writing skills is time-consuming and costly. Integrating AI assessment provides JAEN with a competitive differentiator — delivering instant, detailed feedback that general learning apps do not offer.

**Research directions:**
- Prompt engineering and optimization for language evaluation models
- Asynchronous handling of AI model responses (non-blocking submission pipeline)
- Per-account usage quota configuration (Quota Management) to control API costs

**Expected outcome:** An integrated AI architecture capable of grading, explaining errors, and analyzing grammar within under 5 minutes, with high system stability and cost efficiency.

---

## Core Features

### 1. Course Search & Filter
Users search by keyword, category, or tag (Free, Paid, Popular, Latest). The system ranks and prioritizes highly-rated courses from the community.

### 2. Progress Tracking
Displays a visual completion percentage chart per course. Learners can inspect the completion status of each lesson's quiz and video modules individually.

### 3. Embedded Video Lectures
Each lesson embeds a video uploaded by the Creator to their personal YouTube channel as Unlisted. The platform streams it via YouTube's embed API without exposing direct links.

### 4. AI Assessment (Speaking & Writing)
Learners upload an audio recording (Speaking) or written text (Writing). The AI Engine returns detailed feedback — including pronunciation errors, grammar corrections, and structural suggestions — within under 5 minutes.

### 5. Personal Dictionary
Words highlighted directly in PDF materials can be saved to a personal vocabulary bank. The system automatically syncs and schedules spaced-repetition review sessions.

### 6. Secure Payments
Integrated with PayPal and VNPAY. A minimum transaction value of 75,000 VND applies. All payment fulfillment events are handled via webhook and mapped to enrollment state transitions.

### 7. Moderation & Violation Reporting
Every course and attachment includes a Report button. Content is automatically hidden or flagged for Admin review when report thresholds are exceeded.

### 8. Course Creation Modules
Creators can build rich learning materials using 10 content module types, including Flashcard sets, Multiple Choice Quizzes, Gap-Fill exercises, Reading passages, and Listening activities.

---

## Video & Content Security Strategy

JAEN does not self-host a video storage server (cost and bandwidth prohibitive). Instead, three content delivery cases apply:

- **Case 1 — Video lectures:** Creators upload to their personal YouTube channel as Unlisted. The platform embeds via a secured video ID; direct links are never exposed to learners.
- **Case 2 — Text materials:** PDF documents are rendered directly through an in-platform viewer; files cannot be downloaded by learners.
- **Case 3 — Interactive assets & supplementary files:** All uploads pass through an Authorization Middleware and an automated virus scanner before being made available to learners.

---

## Content Rollout Strategy

| Phase | Focus |
|---|---|
| Layer 1 | Public lecture data, Unlisted YouTube embeds, PDF materials, basic multiple-choice quizzes |
| Layer 2 | Certified Creator partnerships, AI-powered Speaking/Writing grading, premium course publishing |
| Layer 3 | Full marketplace model, automated revenue sharing, real-exam simulation modules |

---

## System State Lifecycles

JAEN defines and monitors behavioral state lifecycles for five critical domain objects:

- **UserAccount** — `PendingVerification` → `Active` → `Inactive` → `Suspended`
- **LearningContent** — `Draft` → `UnderAIReview` → `PendingApproval` → `Published` → `Archived`
- **Assessment** — `Open` → `InProgress` → `Submitted` → `Graded` → `Closed`
- **LearnerEnrollment** — `Enrolled` → `InProgress` → `Completed` / `Failed`
- **Plugin** — `Installed` → `Enabled` → `Disabled` → `Uninstalled`
