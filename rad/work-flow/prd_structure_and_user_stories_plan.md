# PRD Structure & User Stories Plan

## Document Purpose
This document organizes the Business Requirements into a structured PRD format, mapping all epics, features, and user stories for the Medical Exam Platform.

---

## 1. User Roles & Actors

| Role | Description | Access Level |
|------|-------------|--------------|
| **Visitor** | Anonymous user browsing public website | Public pages only |
| **Subscriber** | Active user with material subscription(s) | Portal access for subscribed materials |
| **Researcher** | Content creator/editor | Content management panels only |
| **Salesperson** | Lead manager, quotation handler, subscription activator | CRM dashboard + subscription management |
| **Admin** | Platform administrator | Full system access |

> **Note**: No Trial/Freemium/Premium tiers. Subscription is per-material with duration set by salesperson during sales process.

---

## 2. Business Model: Quotation-Based Sales

### Customer Journey Flow

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                        QUOTATION-BASED SALES FLOW                            │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐              │
│  │ VISITOR  │ →  │ BROWSE   │ →  │ REQUEST  │ →  │  LEAD    │              │
│  │          │    │ MATERIALS│    │ QUOTATION│    │ CREATED  │              │
│  └──────────┘    └──────────┘    └──────────┘    └──────────┘              │
│                                                         ↓                    │
│  ┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐              │
│  │SUBSCRIBER│ ←  │ ACCOUNT  │ ←  │ PAYMENT  │ ←  │SALESPERSON│             │
│  │ ACCESS   │    │ ACTIVATED│    │ CONFIRMED│    │ CONTACTS │              │
│  └──────────┘    └──────────┘    └──────────┘    └──────────┘              │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Key Business Rules

1. **No public pricing** - Visitors cannot see prices or subscription durations
2. **Quotation-based** - Visitors request quotation for specific material(s)
3. **Salesperson-driven** - Salesperson sets price and duration per deal
4. **Material-based subscription** - Each subscription is for specific material + duration
5. **Activation by salesperson** - Account created/activated after payment confirmation

---

## 3. Module/Epic Structure

### Epic Map Overview

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           MEDICAL EXAM PLATFORM                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 1: PUBLIC WEBSITE (Lead Generation)                             │   │
│  │ Actor: Visitor                                                       │   │
│  │ Goal: Showcase value → Capture quotation requests                    │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                    ↓                                         │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 2: AUTHENTICATION & ACCESS                                      │   │
│  │ Actors: Subscriber, Salesperson (activation)                         │   │
│  │ Goal: Secure login for activated subscribers                         │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                    ↓                                         │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 3: SUBSCRIBER PORTAL (Learning Loop)                            │   │
│  │ Actor: Subscriber                                                    │   │
│  │                                                                       │   │
│  │  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐       │   │
│  │  │ 3.1 Materials   │→ │ 3.2 Bank        │→ │ 3.3 Practice/   │       │   │
│  │  │ Dashboard       │  │ Dashboard       │  │ Exam Session    │       │   │
│  │  └─────────────────┘  └─────────────────┘  └─────────────────┘       │   │
│  │           ↑                    ↑                    ↓                 │   │
│  │           └────────────────────┴────────────────────┘                 │   │
│  │                        (Learning Loop)                                │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                                                              │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 4: RESEARCHER DASHBOARD (Content Management)                    │   │
│  │ Actor: Researcher                                                    │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                                                              │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 5: SALESPERSON CRM DASHBOARD (Quotation → Activation)           │   │
│  │ Actor: Salesperson                                                   │   │
│  │ Goal: Handle quotations, negotiate, configure subscription, activate │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                                                              │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │ EPIC 6: ADMIN DASHBOARD                                              │   │
│  │ Actor: Admin                                                         │   │
│  └──────────────────────────────────────────────────────────────────────┘   │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 4. Detailed Epic Breakdown

### EPIC 1: PUBLIC WEBSITE (Lead Generation)

**Goal**: Showcase platform value and capture quotation requests for materials

| Feature | Priority | Description |
|---------|----------|-------------|
| F1.1 Homepage | MVP | Value proposition, key benefits, social proof, CTA to browse materials |
| F1.2 Materials Listing | MVP | Browse available exam preparations (no pricing shown) |
| F1.3 Material Detail | MVP | Description, scope, question count, features included |
| F1.4 Features Page | MVP | Study modes, analytics, notes, search, ranking |
| F1.5 Quotation Request Form | MVP | Request quote for selected material(s) |
| F1.6 Contact/Support | MVP | General inquiries |
| F1.7 Legal Pages | MVP | Terms of Service, Privacy Policy |

**User Stories for Epic 1:**

```
US-1.1.1: As a visitor, I want to see the platform's value proposition on the homepage so that I understand what benefits I'll get.
US-1.1.2: As a visitor, I want to see social proof (testimonials, statistics) so that I trust the platform.
US-1.1.3: As a visitor, I want clear CTAs to browse materials so that I can explore what's available.

US-1.2.1: As a visitor, I want to browse available exam materials so that I can see if my target exam is covered.
US-1.2.2: As a visitor, I want to see material names and categories so that I can find what I need.
US-1.2.3: As a visitor, I want to filter materials by exam type so that I can narrow my search.

US-1.3.1: As a visitor, I want to see material descriptions so that I understand what's included.
US-1.3.2: As a visitor, I want to see the scope of each material so that I know what topics are covered.
US-1.3.3: As a visitor, I want to see question bank counts so that I understand the volume of content.
US-1.3.4: As a visitor, I want to see included features per material so that I know what tools I'll have.

US-1.4.1: As a visitor, I want to understand study modes available so that I know how I'll learn.
US-1.4.2: As a visitor, I want to see analytics features so that I understand how I'll track progress.
US-1.4.3: As a visitor, I want to see notes and search features so that I know I can organize my learning.

US-1.5.1: As a visitor, I want to request a quotation for specific material(s) so that I can get pricing information.
US-1.5.2: As a visitor, I want to provide my contact information in the quotation form so that sales can reach me.
US-1.5.3: As a visitor, I want to select multiple materials in one quotation request so that I can get a bundle price.
US-1.5.4: As a visitor, I want to add a message to my quotation request so that I can explain my needs.
US-1.5.5: As a visitor, I want to receive confirmation that my quotation request was submitted so that I know to expect contact.

US-1.6.1: As a visitor, I want to contact support so that I can ask questions about the platform.

US-1.7.1: As a visitor, I want to read Terms of Service so that I understand the legal agreement.
US-1.7.2: As a visitor, I want to read Privacy Policy so that I understand data handling.
```

---

### EPIC 2: AUTHENTICATION & ACCESS

**Goal**: Secure access for activated subscribers (no self-registration)

| Feature | Priority | Description |
|---------|----------|-------------|
| F2.1 Login | MVP | Email/password authentication |
| F2.2 Logout | MVP | Secure session termination |
| F2.3 Password Reset | MVP | Forgot password via email |
| F2.4 Password Change | MVP | Change password when logged in |
| F2.5 Account Activation | MVP | Salesperson creates account and sends credentials |
| F2.6 My Subscriptions View | MVP | View active material subscriptions and expiry dates |
| F2.7 Social Login | Phase 2 | Google/Facebook authentication |

**User Stories for Epic 2:**

```
US-2.1.1: As a subscriber, I want to login with email/password so that I can access my portal.
US-2.1.2: As a subscriber, I want to see an error if credentials are wrong so that I know to retry.
US-2.1.3: As a subscriber, I want to stay logged in (remember me) so that I don't login repeatedly.

US-2.2.1: As a subscriber, I want to logout so that my session is secure on shared devices.

US-2.3.1: As a subscriber, I want to reset my password via email so that I can regain access if I forget it.
US-2.3.2: As a subscriber, I want to receive a password reset link so that I can create a new password.

US-2.4.1: As a subscriber, I want to change my password so that I can maintain security.

US-2.5.1: As a new user, I want to receive an activation email with credentials so that I can access my subscription.
US-2.5.2: As a new user, I want to set my own password on first login so that my account is secure.

US-2.6.1: As a subscriber, I want to see my active subscriptions so that I know what materials I can access.
US-2.6.2: As a subscriber, I want to see subscription expiry dates so that I know when to renew.
US-2.6.3: As a subscriber, I want to request renewal for expiring subscriptions so that I can continue access.
```

---

### EPIC 3: SUBSCRIBER PORTAL (Learning Loop)

**Goal**: Provide the core learning experience with practice, exams, analytics, and improvement tools

#### Sub-Epic 3.1: Materials Dashboard

| Feature | Priority | Description |
|---------|----------|-------------|
| F3.1.1 My Materials List | MVP | View subscribed materials only |
| F3.1.2 Material Card | MVP | Name, description, activity indicators, expiry date |
| F3.1.3 Subscription Status | MVP | Show active/expiring/expired status |
| F3.1.4 Renewal Request | MVP | Request renewal for expiring subscriptions |

**User Stories:**

```
US-3.1.1: As a subscriber, I want to see all my subscribed materials so that I can choose what to study.
US-3.1.2: As a subscriber, I want to see activity indicators per material so that I know my progress.
US-3.1.3: As a subscriber, I want to see subscription expiry dates so that I can plan my studying.
US-3.1.4: As a subscriber, I want to see subscription status (active/expiring/expired) so that I know my access.
US-3.1.5: As a subscriber, I want to request renewal for expiring materials so that I can continue access.
US-3.1.6: As a subscriber, I want to click a material to enter its dashboard so that I can start studying.
```

---

#### Sub-Epic 3.2: Bank Dashboard (Enhancement Center)

| Feature | Priority | Description |
|---------|----------|-------------|
| F3.2.1 Bank Overview | MVP | Quick summary (attempted/correct/incorrect/skipped) |
| F3.2.2 Bank List | MVP | View all banks within material |
| F3.2.3 Exam History | MVP | List of completed exams/sessions with scores |
| F3.2.4 Start Session | MVP | Entry point to practice/exam |
| F3.2.5 Search Panel | MVP | Find questions, revisit answered questions |
| F3.2.6 Notes Management | MVP | Create, list, jump to question |
| F3.2.7 Tasks Management | MVP | Create, view active/completed tasks |
| F3.2.8 Performance Dashboard | MVP | Analytics, topic breakdown, trends |
| F3.2.9 Peer Benchmarking | MVP | Ranking indicator (above/average/below) |
| F3.2.10 Recommendations | Phase 2 | AI-driven next actions |

**User Stories:**

```
US-3.2.1: As a subscriber, I want to see a quick summary of my bank progress so that I know my overall status.
US-3.2.2: As a subscriber, I want to see all question banks in a material so that I can choose which to practice.
US-3.2.3: As a subscriber, I want to see simple activity indicators per bank so that I know where I've been active.

US-3.2.4: As a subscriber, I want to see my exam history so that I can track my attempts.
US-3.2.5: As a subscriber, I want to see scores and dates for past exams so that I can measure improvement.
US-3.2.6: As a subscriber, I want to start a new practice session so that I can continue learning.
US-3.2.7: As a subscriber, I want to start a new exam so that I can test my knowledge.

US-3.2.8: As a subscriber, I want to search questions by keyword so that I can find specific topics.
US-3.2.9: As a subscriber, I want to revisit previously answered questions so that I can review my work.
US-3.2.10: As a subscriber, I want to filter search by correct/incorrect/flagged so that I focus on problem areas.

US-3.2.11: As a subscriber, I want to create notes during exams so that I can capture insights.
US-3.2.12: As a subscriber, I want to view all my notes in the dashboard so that I can review them.
US-3.2.13: As a subscriber, I want to click a note to jump to its question so that I can see the context.
US-3.2.14: As a subscriber, I want to edit/delete notes so that I can manage my content.

US-3.2.15: As a subscriber, I want to create tasks for myself so that I can track follow-up actions.
US-3.2.16: As a subscriber, I want to view active tasks so that I know what to do next.
US-3.2.17: As a subscriber, I want to mark tasks complete so that I can track my progress.
US-3.2.18: As a subscriber, I want to view completed tasks so that I can see what I've accomplished.

US-3.2.19: As a subscriber, I want to see my performance dashboard so that I understand my strengths/weaknesses.
US-3.2.20: As a subscriber, I want to see topic breakdown analytics so that I know which areas need work.
US-3.2.21: As a subscriber, I want to see trends over time so that I can measure my improvement.
US-3.2.22: As a subscriber, I want to see peer comparison so that I know where I stand vs others.
```

---

#### Sub-Epic 3.3: Practice/Exam Session

| Feature | Priority | Description |
|---------|----------|-------------|
| F3.3.1 Study Mode: Revision/Tutor | MVP | Untimed practice with explanations |
| F3.3.2 Study Mode: Timed Test | MVP | Timed practice session |
| F3.3.3 Study Mode: Mock Exam | MVP | Full exam simulation |
| F3.3.4 Study Mode: Review Mode | MVP | Review incorrect/flagged questions |
| F3.3.5 Question Display | MVP | Question, options, navigation |
| F3.3.6 Answer Submission | MVP | Select answer, confirm |
| F3.3.7 Immediate Feedback | MVP | Show correct/incorrect with explanation |
| F3.3.8 Flag Question | MVP | Mark for later review |
| F3.3.9 Session Notes | MVP | Add notes during session |
| F3.3.10 Session Results | MVP | Summary screen with score, breakdown |
| F3.3.11 Spaced Repetition | Phase 2 | FSRS algorithm integration |
| F3.3.12 Adaptive Learning | Phase 2 | IRT-based question selection |

**User Stories:**

```
US-3.3.1: As a subscriber, I want to choose Revision mode so that I can practice without time pressure.
US-3.3.2: As a subscriber, I want to see explanations immediately after answering so that I learn from mistakes.
US-3.3.3: As a subscriber, I want to choose Timed Test mode so that I can practice under time constraints.
US-3.3.4: As a subscriber, I want to see a timer during timed sessions so that I can manage my time.
US-3.3.5: As a subscriber, I want to choose Mock Exam mode so that I can simulate real exam conditions.
US-3.3.6: As a subscriber, I want to choose Review mode so that I can focus on incorrect/flagged questions.

US-3.3.7: As a subscriber, I want to see a question clearly displayed so that I can read and understand it.
US-3.3.8: As a subscriber, I want to see answer options so that I can make a selection.
US-3.3.9: As a subscriber, I want to navigate between questions so that I can review my answers.
US-3.3.10: As a subscriber, I want to skip questions so that I can return to them later.

US-3.3.11: As a subscriber, I want to submit my answer so that I can see if I'm correct.
US-3.3.12: As a subscriber, I want to see immediate feedback so that I learn in the moment.
US-3.3.13: As a subscriber, I want to see detailed explanations so that I understand the reasoning.

US-3.3.14: As a subscriber, I want to flag questions so that I can review them later.
US-3.3.15: As a subscriber, I want to add notes to a question so that I can capture my thoughts.

US-3.3.16: As a subscriber, I want to see my session results so that I know my score.
US-3.3.17: As a subscriber, I want to see topic breakdown in results so that I know weak areas.
US-3.3.18: As a subscriber, I want to review incorrect answers from results so that I can learn from mistakes.
US-3.3.19: As a subscriber, I want to return to bank dashboard from results so that I can continue my learning loop.
```

---

### EPIC 4: RESEARCHER DASHBOARD (Content Management)

**Goal**: Enable researchers to create and manage all educational content

| Feature | Priority | Description |
|---------|----------|-------------|
| F4.1 Materials CRUD | MVP | Create, read, update, delete materials |
| F4.2 Banks CRUD | MVP | Manage question banks within materials |
| F4.3 Questions CRUD | MVP | Create, edit, delete questions |
| F4.4 Answers CRUD | MVP | Manage answer options per question |
| F4.5 Explanations | MVP | Add detailed explanations |
| F4.6 Topic Tagging | MVP | Tag questions by topic/category |
| F4.7 Bulk Import | Phase 2 | Import questions from CSV/Excel |
| F4.8 Content Review Workflow | Phase 2 | Peer review and approval process |
| F4.9 Version History | Phase 2 | Track changes to content |

**User Stories:**

```
US-4.1.1: As a researcher, I want to create a new material so that I can add exam content.
US-4.1.2: As a researcher, I want to edit material details so that I can update information.
US-4.1.3: As a researcher, I want to view all materials so that I can manage them.
US-4.1.4: As a researcher, I want to delete a material so that I can remove outdated content.

US-4.2.1: As a researcher, I want to create question banks within a material so that I can organize content.
US-4.2.2: As a researcher, I want to edit bank details so that I can update scope/description.
US-4.2.3: As a researcher, I want to reorder banks so that I can control the sequence.
US-4.2.4: As a researcher, I want to delete a bank so that I can remove unnecessary sections.

US-4.3.1: As a researcher, I want to create questions with multiple choice answers so that I can build the question bank.
US-4.3.2: As a researcher, I want to edit questions so that I can fix errors or improve clarity.
US-4.3.3: As a researcher, I want to mark the correct answer so that the system can score responses.
US-4.3.4: As a researcher, I want to add explanations so that users understand the reasoning.
US-4.3.5: As a researcher, I want to tag questions by topic so that analytics can show topic breakdowns.
US-4.3.6: As a researcher, I want to preview questions as users see them so that I can verify formatting.
US-4.3.7: As a researcher, I want to delete questions so that I can remove outdated content.

US-4.4.1: As a researcher, I want to add multiple answer options so that I can create proper MCQs.
US-4.4.2: As a researcher, I want to edit answer options so that I can fix errors.
US-4.4.3: As a researcher, I want to reorder answer options so that I can control display order.
```

---

### EPIC 5: SALESPERSON CRM DASHBOARD (Quotation → Activation)

**Goal**: Handle quotation requests, negotiate deals, configure subscriptions, and activate users

| Feature | Priority | Description |
|---------|----------|-------------|
| F5.1 Quotation Inbox | MVP | View new quotation requests as leads |
| F5.2 Lead Details | MVP | View contact info, requested materials, message |
| F5.3 CRM Pipeline | MVP | Kanban stages (New → Contacted → Negotiating → Payment → Activated) |
| F5.4 Lead Assignment | MVP | Assign leads to salespeople |
| F5.5 Communication Log | MVP | Track calls, emails, notes per lead |
| F5.6 Quotation Configuration | MVP | Set price + duration for each requested material |
| F5.7 Quotation Send | MVP | Send formal quotation to lead (email/PDF) |
| F5.8 Payment Confirmation | MVP | Mark payment received |
| F5.9 Account Creation | MVP | Create user account for lead |
| F5.10 Subscription Activation | MVP | Activate subscription(s) for user |
| F5.11 Activation Email | MVP | Send credentials to new subscriber |
| F5.12 Lead Filters/Search | MVP | Filter by stage, date, salesperson, material |
| F5.13 Renewal Requests | MVP | Handle renewal requests from existing subscribers |
| F5.14 Performance Metrics | Phase 2 | Conversion rates, response times, revenue |

**User Stories:**

```
US-5.1.1: As a salesperson, I want to see new quotation requests in my inbox so that I can follow up quickly.
US-5.1.2: As a salesperson, I want to see which materials were requested so that I know what to quote.
US-5.1.3: As a salesperson, I want to see the lead's message so that I understand their needs.

US-5.2.1: As a salesperson, I want to view lead contact details so that I can reach them.
US-5.2.2: As a salesperson, I want to see lead's email and phone so that I have multiple contact options.
US-5.2.3: As a salesperson, I want to see submission date so that I can prioritize recent leads.

US-5.3.1: As a salesperson, I want to see leads in a Kanban pipeline so that I can manage my workflow.
US-5.3.2: As a salesperson, I want to drag leads between stages so that I can update their status.
US-5.3.3: As a salesperson, I want to see leads grouped by stage so that I know my workload.

US-5.4.1: As a sales manager, I want to assign leads to salespeople so that I can distribute work.
US-5.4.2: As a salesperson, I want to see only my assigned leads so that I can focus on my pipeline.

US-5.5.1: As a salesperson, I want to log communication attempts so that I track my interactions.
US-5.5.2: As a salesperson, I want to add notes to leads so that I remember important details.
US-5.5.3: As a salesperson, I want to schedule follow-ups so that I don't forget to contact leads.

US-5.6.1: As a salesperson, I want to set price for each requested material so that I can create a custom quote.
US-5.6.2: As a salesperson, I want to set subscription duration per material so that I can customize the offer.
US-5.6.3: As a salesperson, I want to see base pricing guidelines so that I quote within acceptable ranges.
US-5.6.4: As a salesperson, I want to add discounts so that I can negotiate deals.
US-5.6.5: As a salesperson, I want to calculate total quote amount so that I can present a clear price.

US-5.7.1: As a salesperson, I want to send a formal quotation to the lead so that they have a document to review.
US-5.7.2: As a salesperson, I want quotations to include all materials, prices, and durations so that it's complete.
US-5.7.3: As a salesperson, I want quotations to have an expiry date so that leads act promptly.

US-5.8.1: As a salesperson, I want to confirm payment received so that I can proceed with activation.
US-5.8.2: As a salesperson, I want to record payment method and reference so that I have audit trail.

US-5.9.1: As a salesperson, I want to create a user account for the lead so that they can access the platform.
US-5.9.2: As a salesperson, I want to enter user details (name, email) so that account is properly set up.

US-5.10.1: As a salesperson, I want to activate subscription(s) for the user so that they gain access.
US-5.10.2: As a salesperson, I want subscriptions to match the quotation (materials + durations) so that it's accurate.
US-5.10.3: As a salesperson, I want to see activation confirmation so that I know it succeeded.

US-5.11.1: As a salesperson, I want to send activation email to user so that they receive their credentials.
US-5.11.2: As a salesperson, I want the email to include login link and temporary password so that user can access immediately.

US-5.12.1: As a salesperson, I want to filter leads by stage so that I can focus on specific groups.
US-5.12.2: As a salesperson, I want to search leads by name/email so that I can find specific users.
US-5.12.3: As a salesperson, I want to filter by material requested so that I can group similar leads.
US-5.12.4: As a salesperson, I want to filter by date so that I can see recent requests.

US-5.13.1: As a salesperson, I want to see renewal requests from existing subscribers so that I can retain customers.
US-5.13.2: As a salesperson, I want to see subscriber's history so that I can offer appropriate renewal terms.
US-5.13.3: As a salesperson, I want to process renewals similar to new subscriptions so that workflow is consistent.
```

---

### EPIC 6: ADMIN DASHBOARD

**Goal**: Full platform control and oversight

| Feature | Priority | Description |
|---------|----------|-------------|
| F6.1 User Management | MVP | View, edit, deactivate users |
| F6.2 Role Management | MVP | Assign roles (subscriber, researcher, salesperson) |
| F6.3 Subscription Override | MVP | Manually grant/revoke/extend subscriptions |
| F6.4 Material Management | MVP | Publish/unpublish materials |
| F6.5 Pricing Guidelines | MVP | Set base prices and discount limits for salespeople |
| F6.6 System Settings | MVP | Global configuration |
| F6.7 Analytics Overview | MVP | Platform-wide metrics |
| F6.8 Audit Logs | Phase 2 | Track admin and salesperson actions |
| F6.9 Bulk Operations | Phase 2 | Mass user actions |
| F6.10 Revenue Reports | Phase 2 | Financial dashboards |

**User Stories:**

```
US-6.1.1: As an admin, I want to view all users so that I can manage the user base.
US-6.1.2: As an admin, I want to search users by name/email so that I can find specific accounts.
US-6.1.3: As an admin, I want to edit user details so that I can fix errors or update info.
US-6.1.4: As an admin, I want to deactivate users so that I can handle violations or requests.
US-6.1.5: As an admin, I want to reactivate users so that I can restore access when appropriate.

US-6.2.1: As an admin, I want to assign roles to users so that I can control access levels.
US-6.2.2: As an admin, I want to revoke roles so that I can remove access when needed.
US-6.2.3: As an admin, I want to see all users by role so that I can manage team access.

US-6.3.1: As an admin, I want to manually grant subscriptions so that I can handle special cases.
US-6.3.2: As an admin, I want to revoke subscriptions so that I can handle refunds or issues.
US-6.3.3: As an admin, I want to extend subscriptions so that I can accommodate user requests.

US-6.4.1: As an admin, I want to publish materials so that they become visible on public site.
US-6.4.2: As an admin, I want to unpublish materials so that I can hide them from public.
US-6.4.3: As an admin, I want to see material status so that I know what's live.

US-6.5.1: As an admin, I want to set base prices per material so that salespeople have pricing guidelines.
US-6.5.2: As an admin, I want to set maximum discount limits so that salespeople don't undercut too much.
US-6.5.3: As an admin, I want to set default subscription durations so that there's consistency.

US-6.6.1: As an admin, I want to configure global settings so that I can control platform behavior.

US-6.7.1: As an admin, I want to see platform-wide analytics so that I understand overall performance.
US-6.7.2: As an admin, I want to see quotation-to-activation conversion rates so that I can measure sales effectiveness.
US-6.7.3: As an admin, I want to see active subscriber counts so that I can track growth.
US-6.7.4: As an admin, I want to see revenue trends so that I can monitor business health.
```

---

## 5. MVP vs Phase 2 Summary

### MVP Features (Competitive Launch)

| Epic | Features |
|------|----------|
| Epic 1: Public Website | Homepage, Materials Listing/Detail, Features, Quotation Request, Contact, Legal |
| Epic 2: Auth & Access | Login, Logout, Password Reset/Change, Account Activation, My Subscriptions |
| Epic 3: Subscriber Portal | Materials Dashboard, Bank Dashboard, 4 Study Modes, Analytics, Notes, Tasks, Search, Peer Ranking |
| Epic 4: Researcher Dashboard | Full CRUD for Materials, Banks, Questions, Answers, Explanations, Topic Tagging |
| Epic 5: Salesperson CRM | Quotation Inbox, Pipeline, Communication, Quote Config/Send, Payment, Account Creation, Activation, Renewals |
| Epic 6: Admin Dashboard | User Mgmt, Role Mgmt, Subscription Override, Material Publish, Pricing Guidelines, Settings, Analytics |

### Phase 2 Features (Differentiators)

| Epic | Features |
|------|----------|
| Epic 2 | Social Login (Google/Facebook) |
| Epic 3 | Spaced Repetition (FSRS), Adaptive Learning (IRT), AI Recommendations |
| Epic 4 | Bulk Import, Content Review Workflow, Version History |
| Epic 5 | Performance Metrics (conversion, revenue) |
| Epic 6 | Audit Logs, Bulk Operations, Revenue Reports |

### Phase 3 Features (Expansion)

- Gamification/Leaderboards
- Discussion per question / Community features
- Advanced exports, calendar planning
- Institutional admin dashboards
- Native mobile app + offline mode
- Full AI tutor / chat

---

## 6. PRD Writing Order (Recommended)

To ensure dependencies are handled correctly, write PRDs in this order:

```
1. Epic 4: Researcher Dashboard (Content First)
   └── Content must exist before anything else works

2. Epic 6: Admin Dashboard (Platform Control)
   └── Pricing guidelines needed for sales, material publishing needed

3. Epic 5: Salesperson CRM Dashboard (Sales Pipeline)
   └── Core business flow: quotation → activation

4. Epic 2: Authentication & Access (User Foundation)
   └── Depends on salesperson activating accounts

5. Epic 1: Public Website (Lead Generation)
   └── Depends on understanding what materials exist to showcase

6. Epic 3: Subscriber Portal (Core Product)
   └── The main user experience, activated users enter here
```

---

## 7. User Story Template

Use this format for all user stories:

```markdown
### US-[Epic].[Feature].[Story]: [Title]

**As a** [role]
**I want to** [action]
**So that** [benefit]

**Acceptance Criteria:**
- [ ] Given [context], when [action], then [outcome]
- [ ] Given [context], when [action], then [outcome]

**Priority:** MVP | Phase 2 | Phase 3
**Estimate:** [Story Points]
**Dependencies:** [US-X.X.X, US-Y.Y.Y]
```

---

## 8. Data Model Entities (High-Level)

| Entity | Description | Epic |
|--------|-------------|------|
| User | Platform users with roles | 2, 5, 6 |
| Subscription | Material + Duration + Price for a user | 2, 5, 6 |
| Material | Exam preparation materials (e.g., MRCP Part 1) | 1, 3, 4 |
| Bank | Question bank within material | 3, 4 |
| Question | Individual MCQ question | 3, 4 |
| Answer | Answer option for question | 3, 4 |
| Session | Practice/exam session instance | 3 |
| Response | User's answer to a question | 3 |
| Note | User notes attached to questions | 3 |
| Task | User-created tasks | 3 |
| Flag | User flags on questions | 3 |
| Lead | Quotation request / CRM lead record | 5 |
| Quotation | Formal quote with materials, prices, durations | 5 |
| Communication | Lead interaction log | 5 |
| PricingGuideline | Base prices and discount limits per material | 6 |

---

## 9. Key Business Flow Summary

```
┌────────────────────────────────────────────────────────────────────────────┐
│                         COMPLETE BUSINESS FLOW                              │
├────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  PUBLIC WEBSITE                    SALESPERSON CRM                          │
│  ─────────────                     ──────────────                           │
│  1. Visitor browses materials      4. Salesperson sees lead                 │
│  2. Visitor requests quotation     5. Salesperson contacts lead             │
│  3. Lead created in CRM        →   6. Salesperson configures quote          │
│                                    7. Salesperson sends quotation           │
│                                    8. Lead confirms / negotiates            │
│                                    9. Payment received                      │
│                                   10. Salesperson creates account           │
│                                   11. Salesperson activates subscription    │
│                                   12. Activation email sent                 │
│                                                                             │
│  SUBSCRIBER PORTAL                                                          │
│  ────────────────                                                           │
│  13. Subscriber logs in                                                     │
│  14. Subscriber sees materials dashboard                                    │
│  15. Subscriber enters bank dashboard                                       │
│  16. Subscriber practices / takes exams                                     │
│  17. Subscriber reviews results / analytics                                 │
│  18. Learning loop continues...                                             │
│                                                                             │
│  RENEWAL FLOW                                                               │
│  ────────────                                                               │
│  19. Subscription approaching expiry                                        │
│  20. Subscriber requests renewal (from portal)                              │
│  21. Renewal request appears in CRM                                         │
│  22. Salesperson processes renewal (same flow as new)                       │
│                                                                             │
└────────────────────────────────────────────────────────────────────────────┘
```

---

## 10. Next Steps

1. **Review this plan** with stakeholders for approval
2. **Write detailed PRD** for Epic 4 (Researcher Dashboard) first
3. **Create database schema** based on data model entities
4. **Set up Django project** with content models foundation
5. **Iterate** through remaining epics in recommended order

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-26 | Claude | Initial PRD structure and user stories plan |
| 2.0 | 2025-12-26 | Claude | Revised for quotation-based sales model (removed tiers, pricing page, self-checkout) |
