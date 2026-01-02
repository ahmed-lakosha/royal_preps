# Prototype Team Subagents Specification

## Document Purpose
This document defines each team member role as a "subagent" with clear specifications for creating HTML prototype pages for the Medical Exam Platform.

---

## 1. Subagent Architecture Overview

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                        PROTOTYPE TEAM SUBAGENTS                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│                    ┌─────────────────────────┐                               │
│                    │   PROJECT COORDINATOR   │                               │
│                    │       (Optional)        │                               │
│                    │                         │                               │
│                    │  • Task assignment      │                               │
│                    │  • Progress tracking    │                               │
│                    │  • Quality gates        │                               │
│                    └───────────┬─────────────┘                               │
│                                │                                             │
│              ┌─────────────────┴─────────────────┐                           │
│              │                                   │                           │
│              ▼                                   ▼                           │
│  ┌─────────────────────────┐     ┌─────────────────────────┐                │
│  │    UI/UX DESIGNER       │     │   FRONTEND DEVELOPER    │                │
│  │                         │     │                         │                │
│  │  • Wireframes           │────▶│  • HTML structure       │                │
│  │  • Visual design        │     │  • CSS/SCSS styling     │                │
│  │  • Design system        │     │  • JS interactions      │                │
│  │  • Component library    │     │  • Responsive layout    │                │
│  │  • User flows           │     │  • Component assembly   │                │
│  └─────────────────────────┘     └─────────────────────────┘                │
│                                                                              │
│              INPUT                              OUTPUT                       │
│              ─────                              ──────                       │
│              PRD Document                       HTML Prototype Pages         │
│              User Stories                       Interactive Preview          │
│              Business Flow                      Clickable Navigation         │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 2. SUBAGENT 1: UI/UX Designer

### 2.1 Identity

| Attribute | Value |
|-----------|-------|
| **Role Name** | UI/UX Designer |
| **Agent ID** | `AGENT-UX-001` |
| **Type** | Creative / Design |
| **Priority** | Primary (starts first) |

### 2.2 Mission Statement

> Design intuitive, visually consistent user interfaces for all platform screens, ensuring excellent user experience across all user roles (Visitor, Subscriber, Researcher, Salesperson, Admin).

### 2.3 Input Requirements

| Input | Source | Format | Required |
|-------|--------|--------|----------|
| PRD Document | Project Files | Markdown | ✅ Yes |
| User Stories | PRD | Text | ✅ Yes |
| Business Flow | PRD | Diagram | ✅ Yes |
| Brand Guidelines | Client | PDF/Figma | ⚠️ If exists |
| Competitor Screenshots | Research | Images | 📌 Optional |
| Content Samples | Client | Text | 📌 Optional |

### 2.4 Core Competencies

```
REQUIRED SKILLS:
├── Design Tools
│   ├── Figma (Primary) ........................ Expert
│   ├── Adobe XD ............................... Intermediate
│   └── Sketch ................................. Intermediate
│
├── Design Disciplines
│   ├── Wireframing ............................ Expert
│   ├── UI Design .............................. Expert
│   ├── UX Design .............................. Expert
│   ├── Design Systems ......................... Advanced
│   ├── Component Libraries .................... Advanced
│   └── Responsive Design ...................... Expert
│
├── Domain Knowledge
│   ├── Dashboard UX Patterns .................. Advanced
│   ├── Form Design ............................ Advanced
│   ├── Data Visualization ..................... Intermediate
│   ├── CRM Interface Patterns ................. Intermediate
│   └── E-learning Platform UX ................. Intermediate
│
└── Soft Skills
    ├── Attention to Detail .................... Expert
    ├── Communication .......................... Advanced
    └── Iteration Based on Feedback ............ Advanced
```

### 2.5 Output Deliverables

| Deliverable | Format | Description |
|-------------|--------|-------------|
| **Wireframes** | Figma | Low-fidelity layouts for all screens |
| **UI Mockups** | Figma | High-fidelity visual designs |
| **Design System** | Figma | Colors, typography, spacing, components |
| **Component Library** | Figma | Reusable UI components |
| **User Flows** | Figma | Navigation paths and interactions |
| **Prototype** | Figma | Clickable prototype for review |
| **Design Specs** | Figma/PDF | Measurements, colors, fonts for developers |
| **Asset Export** | PNG/SVG | Icons, images, logos |

### 2.6 Task Breakdown by Epic

#### Phase 1: Foundation (Week 1)

| Task ID | Task | Output | Priority |
|---------|------|--------|----------|
| UX-001 | Create Design System | Colors, typography, spacing tokens | Critical |
| UX-002 | Design Component Library | Buttons, inputs, cards, tables, modals | Critical |
| UX-003 | Define Grid System | 12-column responsive grid | Critical |
| UX-004 | Create Icon Set | 50+ UI icons | High |

#### Phase 2: Public Website (Week 1-2)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-010 | Homepage Design | 1 screen (desktop + mobile) | Critical |
| UX-011 | Materials Listing | 1 screen | Critical |
| UX-012 | Material Detail | 1 screen | Critical |
| UX-013 | Features Page | 1 screen | High |
| UX-014 | Quotation Request Form | 1 screen + success state | Critical |
| UX-015 | Contact Page | 1 screen | Medium |
| UX-016 | Legal Pages | 2 screens (Terms, Privacy) | Low |

#### Phase 3: Authentication (Week 2)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-020 | Login Page | 1 screen + error states | Critical |
| UX-021 | Password Reset | 2 screens (request + set new) | High |
| UX-022 | First Login Set Password | 1 screen | High |
| UX-023 | My Subscriptions View | 1 screen | High |

#### Phase 4: Subscriber Portal (Week 2-3)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-030 | Materials Dashboard | 1 screen | Critical |
| UX-031 | Bank Dashboard | 1 screen (complex) | Critical |
| UX-032 | Study Mode Selection | 1 screen/modal | Critical |
| UX-033 | Question Screen | 1 screen + states | Critical |
| UX-034 | Exam Timer Component | 1 component | High |
| UX-035 | Session Results | 1 screen | Critical |
| UX-036 | Notes Panel | 1 panel/sidebar | High |
| UX-037 | Tasks Panel | 1 panel/sidebar | High |
| UX-038 | Search Panel | 1 panel/modal | High |
| UX-039 | Analytics Dashboard | 1 screen (charts) | High |
| UX-040 | Peer Ranking Component | 1 component | Medium |

#### Phase 5: Researcher Dashboard (Week 3)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-050 | Materials List | 1 screen | Critical |
| UX-051 | Material Create/Edit Form | 1 screen | Critical |
| UX-052 | Banks List | 1 screen | Critical |
| UX-053 | Bank Create/Edit Form | 1 screen | Critical |
| UX-054 | Questions List | 1 screen | Critical |
| UX-055 | Question Create/Edit Form | 1 screen (complex) | Critical |
| UX-056 | Question Preview | 1 modal/screen | High |
| UX-057 | Bulk Actions UI | 1 component | Medium |

#### Phase 6: Salesperson CRM (Week 3-4)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-060 | Lead Inbox/List | 1 screen | Critical |
| UX-061 | Kanban Pipeline | 1 screen | Critical |
| UX-062 | Lead Detail View | 1 screen | Critical |
| UX-063 | Communication Log | 1 panel | High |
| UX-064 | Quotation Configuration | 1 screen/modal | Critical |
| UX-065 | Quotation Preview/PDF | 1 screen | Critical |
| UX-066 | Account Creation Form | 1 modal | High |
| UX-067 | Subscription Activation | 1 modal | High |
| UX-068 | Filters & Search | 1 panel | Medium |
| UX-069 | Renewal Request View | 1 screen | High |

#### Phase 7: Admin Dashboard (Week 4)

| Task ID | Task | Screens | Priority |
|---------|------|---------|----------|
| UX-070 | Admin Overview/Home | 1 screen | High |
| UX-071 | Users List | 1 screen | Critical |
| UX-072 | User Edit Form | 1 modal/screen | Critical |
| UX-073 | Role Management | 1 screen | High |
| UX-074 | Subscription Management | 1 screen | High |
| UX-075 | Material Publish Control | 1 screen | High |
| UX-076 | Pricing Guidelines | 1 screen | High |
| UX-077 | System Settings | 1 screen | Medium |
| UX-078 | Platform Analytics | 1 screen | High |

### 2.7 Quality Criteria

```
ACCEPTANCE CRITERIA FOR UI/UX DELIVERABLES:

□ All screens match the PRD requirements
□ Consistent use of design system across all screens
□ Responsive designs for desktop (1440px, 1280px) and mobile (375px)
□ All interactive states defined (hover, active, disabled, error, success)
□ All empty states designed (no data, loading, error)
□ Accessibility considerations (contrast, font sizes)
□ Clickable prototype covers main user flows
□ Design specs exported for developer handoff
□ All assets exported in correct formats (SVG for icons, PNG for images)
```

### 2.8 Interaction with Other Subagents

| Interacts With | Direction | What |
|----------------|-----------|------|
| Project Coordinator | ← Receives | Task priorities, feedback |
| Project Coordinator | → Sends | Progress updates, blockers |
| Frontend Developer | → Sends | Design files, specs, assets |
| Frontend Developer | ← Receives | Feasibility feedback, questions |

---

## 3. SUBAGENT 2: Frontend Developer

### 3.1 Identity

| Attribute | Value |
|-----------|-------|
| **Role Name** | Frontend Developer |
| **Agent ID** | `AGENT-FE-001` |
| **Type** | Technical / Development |
| **Priority** | Secondary (starts after UX Phase 1) |

### 3.2 Mission Statement

> Convert UI/UX designs into functional, responsive HTML prototype pages with CSS styling and JavaScript interactions, creating a realistic preview of the final platform.

### 3.3 Input Requirements

| Input | Source | Format | Required |
|-------|--------|--------|----------|
| UI Mockups | UI/UX Designer | Figma | ✅ Yes |
| Design System | UI/UX Designer | Figma | ✅ Yes |
| Component Library | UI/UX Designer | Figma | ✅ Yes |
| Design Specs | UI/UX Designer | Figma/PDF | ✅ Yes |
| Assets (icons, images) | UI/UX Designer | SVG/PNG | ✅ Yes |
| PRD Document | Project Files | Markdown | ✅ Yes |
| Sample Content | Client | Text/JSON | 📌 Optional |

### 3.4 Core Competencies

```
REQUIRED SKILLS:
├── Core Technologies
│   ├── HTML5 ................................. Expert
│   ├── CSS3 .................................. Expert
│   ├── SCSS/SASS ............................. Advanced
│   ├── JavaScript (ES6+) ..................... Advanced
│   └── Responsive Design ..................... Expert
│
├── Frameworks & Libraries
│   ├── Bootstrap 5 OR Tailwind CSS ........... Advanced
│   ├── jQuery (optional) ..................... Intermediate
│   ├── Chart.js (for analytics) .............. Intermediate
│   └── Sortable.js (for Kanban) .............. Intermediate
│
├── Development Tools
│   ├── VS Code ............................... Expert
│   ├── Git .................................. Advanced
│   ├── Browser DevTools ...................... Expert
│   ├── Figma (for inspection) ................ Intermediate
│   └── npm/yarn ............................. Intermediate
│
├── Best Practices
│   ├── Semantic HTML ......................... Expert
│   ├── BEM Naming Convention ................. Advanced
│   ├── CSS Variables ......................... Advanced
│   ├── Mobile-First Approach ................. Advanced
│   └── Cross-Browser Compatibility ........... Advanced
│
└── Soft Skills
    ├── Attention to Detail ................... Expert
    ├── Design Interpretation ................. Advanced
    └── Problem Solving ....................... Advanced
```

### 3.5 Output Deliverables

| Deliverable | Format | Description |
|-------------|--------|-------------|
| **HTML Pages** | .html | All prototype screens |
| **CSS/SCSS Files** | .css/.scss | Styling with design system |
| **JavaScript Files** | .js | Interactions and behaviors |
| **Assets Folder** | /assets | Images, icons, fonts |
| **Component Library** | /components | Reusable HTML components |
| **Documentation** | README.md | How to run/view prototype |

### 3.6 Project Structure

```
medical-exam-prototype/
├── index.html                      # Homepage
├── README.md                       # Documentation
│
├── assets/
│   ├── css/
│   │   ├── main.css               # Compiled CSS
│   │   └── main.css.map           # Source map
│   ├── scss/
│   │   ├── main.scss              # Main SCSS entry
│   │   ├── _variables.scss        # Design tokens
│   │   ├── _mixins.scss           # SCSS mixins
│   │   ├── _reset.scss            # CSS reset
│   │   ├── _typography.scss       # Font styles
│   │   ├── _buttons.scss          # Button components
│   │   ├── _forms.scss            # Form components
│   │   ├── _cards.scss            # Card components
│   │   ├── _tables.scss           # Table components
│   │   ├── _modals.scss           # Modal components
│   │   ├── _navigation.scss       # Nav components
│   │   └── _utilities.scss        # Utility classes
│   ├── js/
│   │   ├── main.js                # Main JavaScript
│   │   ├── navigation.js          # Navigation logic
│   │   ├── modals.js              # Modal interactions
│   │   ├── forms.js               # Form validation
│   │   ├── charts.js              # Chart initialization
│   │   └── kanban.js              # Kanban drag-drop
│   ├── images/
│   │   ├── logo.svg
│   │   ├── icons/                 # Icon sprites
│   │   └── placeholders/          # Placeholder images
│   └── fonts/                     # Custom fonts if any
│
├── public/                        # Public website pages
│   ├── index.html                 # Homepage
│   ├── materials.html             # Materials listing
│   ├── material-detail.html       # Material detail
│   ├── features.html              # Features page
│   ├── quotation.html             # Quotation request
│   ├── contact.html               # Contact page
│   ├── terms.html                 # Terms of Service
│   └── privacy.html               # Privacy Policy
│
├── auth/                          # Authentication pages
│   ├── login.html                 # Login page
│   ├── forgot-password.html       # Password reset request
│   ├── reset-password.html        # Set new password
│   └── first-login.html           # First login set password
│
├── subscriber/                    # Subscriber portal
│   ├── dashboard.html             # Materials dashboard
│   ├── bank-dashboard.html        # Bank dashboard
│   ├── exam-setup.html            # Study mode selection
│   ├── question.html              # Question screen
│   ├── results.html               # Session results
│   ├── analytics.html             # Performance analytics
│   ├── notes.html                 # Notes view
│   ├── tasks.html                 # Tasks view
│   ├── search.html                # Search view
│   └── subscriptions.html         # My subscriptions
│
├── researcher/                    # Researcher dashboard
│   ├── dashboard.html             # Overview
│   ├── materials.html             # Materials list
│   ├── material-form.html         # Create/edit material
│   ├── banks.html                 # Banks list
│   ├── bank-form.html             # Create/edit bank
│   ├── questions.html             # Questions list
│   ├── question-form.html         # Create/edit question
│   └── question-preview.html      # Preview question
│
├── sales/                         # Salesperson CRM
│   ├── dashboard.html             # CRM overview
│   ├── leads.html                 # Lead inbox/list
│   ├── pipeline.html              # Kanban pipeline
│   ├── lead-detail.html           # Lead detail view
│   ├── quotation.html             # Quotation configuration
│   ├── quotation-preview.html     # Quotation preview
│   └── renewals.html              # Renewal requests
│
├── admin/                         # Admin dashboard
│   ├── dashboard.html             # Admin overview
│   ├── users.html                 # Users list
│   ├── user-form.html             # User edit
│   ├── roles.html                 # Role management
│   ├── subscriptions.html         # Subscription management
│   ├── materials.html             # Material publish control
│   ├── pricing.html               # Pricing guidelines
│   ├── settings.html              # System settings
│   └── analytics.html             # Platform analytics
│
└── components/                    # Reusable components
    ├── header-public.html         # Public site header
    ├── header-portal.html         # Portal header
    ├── sidebar.html               # Dashboard sidebar
    ├── footer.html                # Footer
    ├── modal-template.html        # Modal template
    ├── card-material.html         # Material card
    ├── card-bank.html             # Bank card
    ├── table-template.html        # Table template
    └── form-elements.html         # Form elements
```

### 3.7 Task Breakdown by Epic

#### Phase 1: Setup & Foundation (Week 1)

| Task ID | Task | Output | Priority |
|---------|------|--------|----------|
| FE-001 | Project Setup | Folder structure, package.json | Critical |
| FE-002 | SCSS Setup | Variables, mixins, reset | Critical |
| FE-003 | Design Tokens Implementation | Colors, typography, spacing | Critical |
| FE-004 | Grid System | Responsive grid classes | Critical |
| FE-005 | Base Components | Buttons, inputs, cards | Critical |
| FE-006 | Navigation Components | Header, sidebar, footer | Critical |
| FE-007 | Modal Component | Reusable modal | High |
| FE-008 | Table Component | Reusable table | High |

#### Phase 2: Public Website (Week 2)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-010 | Homepage | 1 page | Critical |
| FE-011 | Materials Listing | 1 page | Critical |
| FE-012 | Material Detail | 1 page | Critical |
| FE-013 | Features Page | 1 page | High |
| FE-014 | Quotation Form | 1 page + validation | Critical |
| FE-015 | Contact Page | 1 page | Medium |
| FE-016 | Legal Pages | 2 pages | Low |
| FE-017 | Public Navigation | Header + footer | Critical |

#### Phase 3: Authentication (Week 2)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-020 | Login Page | 1 page + states | Critical |
| FE-021 | Forgot Password | 1 page | High |
| FE-022 | Reset Password | 1 page | High |
| FE-023 | First Login | 1 page | High |
| FE-024 | Form Validation JS | validation.js | High |

#### Phase 4: Subscriber Portal (Week 2-3)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-030 | Portal Layout | Sidebar + header | Critical |
| FE-031 | Materials Dashboard | 1 page | Critical |
| FE-032 | Bank Dashboard | 1 page (complex) | Critical |
| FE-033 | Study Mode Selection | 1 modal/page | Critical |
| FE-034 | Question Screen | 1 page + states | Critical |
| FE-035 | Timer Component | JS timer | High |
| FE-036 | Session Results | 1 page | Critical |
| FE-037 | Notes Panel | Panel component | High |
| FE-038 | Tasks Panel | Panel component | High |
| FE-039 | Search Panel | Panel + filters | High |
| FE-040 | Analytics Page | Charts integration | High |
| FE-041 | Subscriptions View | 1 page | High |

#### Phase 5: Researcher Dashboard (Week 3)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-050 | Researcher Layout | Sidebar variant | Critical |
| FE-051 | Materials List | 1 page | Critical |
| FE-052 | Material Form | 1 page | Critical |
| FE-053 | Banks List | 1 page | Critical |
| FE-054 | Bank Form | 1 page | Critical |
| FE-055 | Questions List | 1 page | Critical |
| FE-056 | Question Form | 1 page (complex) | Critical |
| FE-057 | Question Preview | 1 modal | High |
| FE-058 | Rich Text Editor | Integration | Medium |

#### Phase 6: Salesperson CRM (Week 3-4)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-060 | CRM Layout | Sidebar variant | Critical |
| FE-061 | Lead Inbox | 1 page | Critical |
| FE-062 | Kanban Pipeline | 1 page + drag-drop | Critical |
| FE-063 | Lead Detail | 1 page | Critical |
| FE-064 | Communication Log | Panel component | High |
| FE-065 | Quotation Config | 1 modal/page | Critical |
| FE-066 | Quotation Preview | 1 page (printable) | Critical |
| FE-067 | Account Creation | 1 modal | High |
| FE-068 | Activation Modal | 1 modal | High |
| FE-069 | Filters Component | Filter panel | Medium |
| FE-070 | Renewals View | 1 page | High |

#### Phase 7: Admin Dashboard (Week 4)

| Task ID | Task | Pages | Priority |
|---------|------|-------|----------|
| FE-070 | Admin Layout | Sidebar variant | Critical |
| FE-071 | Admin Overview | 1 page | High |
| FE-072 | Users List | 1 page | Critical |
| FE-073 | User Form | 1 modal/page | Critical |
| FE-074 | Roles Page | 1 page | High |
| FE-075 | Subscriptions Page | 1 page | High |
| FE-076 | Materials Publish | 1 page | High |
| FE-077 | Pricing Page | 1 page | High |
| FE-078 | Settings Page | 1 page | Medium |
| FE-079 | Analytics Page | 1 page + charts | High |

### 3.8 Quality Criteria

```
ACCEPTANCE CRITERIA FOR FRONTEND DELIVERABLES:

□ Pixel-perfect implementation of designs (±2px tolerance)
□ All pages responsive (desktop, tablet, mobile)
□ Consistent use of design system variables
□ No inline styles (all in SCSS files)
□ No inline scripts (all in JS files)
□ Semantic HTML structure
□ All interactive elements functional (navigation, modals, tabs)
□ Form validation working
□ Cross-browser tested (Chrome, Firefox, Safari, Edge)
□ No console errors
□ Fast page load (< 3s on standard connection)
□ All links working between pages
□ Mock data populated in all screens
```

### 3.9 Interaction with Other Subagents

| Interacts With | Direction | What |
|----------------|-----------|------|
| UI/UX Designer | ← Receives | Design files, specs, assets |
| UI/UX Designer | → Sends | Questions, feasibility feedback |
| Project Coordinator | ← Receives | Task priorities, deadlines |
| Project Coordinator | → Sends | Progress updates, blockers |

---

## 4. SUBAGENT 3: Project Coordinator (Optional)

### 4.1 Identity

| Attribute | Value |
|-----------|-------|
| **Role Name** | Project Coordinator |
| **Agent ID** | `AGENT-PM-001` |
| **Type** | Management / Coordination |
| **Priority** | Support (throughout project) |

### 4.2 Mission Statement

> Coordinate the prototype development process, ensuring timely delivery, quality standards, and effective communication between subagents.

### 4.3 Core Responsibilities

```
COORDINATION TASKS:
├── Planning
│   ├── Break down PRD into tasks
│   ├── Create timeline/schedule
│   ├── Assign tasks to subagents
│   └── Define milestones
│
├── Tracking
│   ├── Monitor task progress
│   ├── Identify blockers
│   ├── Update task status
│   └── Report to stakeholders
│
├── Quality
│   ├── Review deliverables
│   ├── Ensure consistency
│   ├── Coordinate feedback
│   └── Sign off on milestones
│
└── Communication
    ├── Daily standups (async)
    ├── Clarify requirements
    ├── Resolve conflicts
    └── Stakeholder updates
```

### 4.4 Tools & Methods

| Tool | Purpose |
|------|---------|
| Task Board | Track tasks (Trello, Notion, Azure DevOps) |
| Timeline | Gantt chart or calendar view |
| Communication | Slack, Teams, or async updates |
| Documentation | Confluence, Notion, or Markdown |
| Version Control | Git for file versioning |

---

## 5. Subagent Interaction Workflow

### 5.1 Sequential Flow

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                        PROTOTYPE DEVELOPMENT WORKFLOW                        │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  WEEK 1                                                                      │
│  ──────                                                                      │
│  ┌─────────────┐                                                            │
│  │  UX-001     │  UI/UX Designer: Design System                             │
│  │  to         │  ────────────────────────────                              │
│  │  UX-004     │  Colors, Typography, Components, Icons                     │
│  └──────┬──────┘                                                            │
│         │                                                                    │
│         ▼                                                                    │
│  ┌─────────────┐                                                            │
│  │  FE-001     │  Frontend Developer: Setup & Foundation                    │
│  │  to         │  ──────────────────────────────────                        │
│  │  FE-008     │  Project setup, SCSS, Base components                      │
│  └─────────────┘                                                            │
│                                                                              │
│  WEEK 2                                                                      │
│  ──────                                                                      │
│  ┌─────────────┐         ┌─────────────┐                                    │
│  │  UX-010     │         │  FE-010     │                                    │
│  │  to         │ ──────▶ │  to         │  Public Website Pages              │
│  │  UX-023     │         │  FE-024     │                                    │
│  └─────────────┘         └─────────────┘                                    │
│  UI/UX: Public +         Frontend: Build                                    │
│  Auth designs            pages as designs                                   │
│                          are delivered                                      │
│                                                                              │
│  WEEK 3                                                                      │
│  ──────                                                                      │
│  ┌─────────────┐         ┌─────────────┐                                    │
│  │  UX-030     │         │  FE-030     │                                    │
│  │  to         │ ──────▶ │  to         │  Portal + Researcher Pages         │
│  │  UX-057     │         │  FE-058     │                                    │
│  └─────────────┘         └─────────────┘                                    │
│                                                                              │
│  WEEK 4                                                                      │
│  ──────                                                                      │
│  ┌─────────────┐         ┌─────────────┐                                    │
│  │  UX-060     │         │  FE-060     │                                    │
│  │  to         │ ──────▶ │  to         │  CRM + Admin Pages                 │
│  │  UX-078     │         │  FE-079     │                                    │
│  └─────────────┘         └─────────────┘                                    │
│                                                                              │
│  WEEK 5 (Buffer)                                                             │
│  ──────────────                                                              │
│  ┌─────────────────────────────────────────────────────────────────────┐    │
│  │  Review, Fixes, Polish, Final Delivery                               │    │
│  └─────────────────────────────────────────────────────────────────────┘    │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

### 5.2 Parallel Execution Strategy

```
PARALLEL WORK OPPORTUNITIES:

Week 2:
├── UX: Designing Subscriber Portal screens
├── FE: Building Public Website + Auth (from Week 1 designs)
└── Parallel efficiency: 80%

Week 3:
├── UX: Designing CRM + Admin screens
├── FE: Building Subscriber Portal + Researcher (from Week 2 designs)
└── Parallel efficiency: 85%

Week 4:
├── UX: Review and refinements
├── FE: Building CRM + Admin (from Week 3 designs)
└── Parallel efficiency: 90%
```

---

## 6. Handoff Protocol

### 6.1 UX → Frontend Handoff Checklist

```
DESIGN HANDOFF REQUIREMENTS:

□ Figma file organized by pages/sections
□ All components in component library
□ Design tokens documented
  □ Colors (with HEX values)
  □ Typography (font family, sizes, weights)
  □ Spacing (margin, padding values)
  □ Border radius values
  □ Shadow values
□ Responsive breakpoints defined
□ Interactive states shown (hover, active, disabled, error)
□ Empty states designed
□ Loading states designed
□ Assets exported
  □ Icons as SVG
  □ Images as PNG/WebP
  □ Logo variants
□ Prototype clickable for reference
□ Notes/annotations for complex interactions
```

### 6.2 Communication Protocol

| Event | From | To | Method |
|-------|------|-----|--------|
| Design ready for section | UX | FE | Notification + Link |
| Question about design | FE | UX | Direct message |
| Design change needed | FE | UX | Request + Reason |
| Task completed | Any | PM | Status update |
| Blocker identified | Any | PM | Immediate alert |
| Milestone complete | PM | All | Announcement |

---

## 7. Timeline Summary

| Week | UI/UX Designer | Frontend Developer | Milestone |
|------|----------------|-------------------|-----------|
| 1 | Design System, Components, Icons | Setup, SCSS, Base Components | Foundation Complete |
| 2 | Public Website, Auth designs | Public Website, Auth pages | Public Site Complete |
| 3 | Portal, Researcher designs | Portal, Researcher pages | Subscriber Flow Complete |
| 4 | CRM, Admin designs | CRM, Admin pages | All Dashboards Complete |
| 5 | Review, Polish | Fixes, Responsive | Prototype Delivered |

---

## 8. Success Metrics

| Metric | Target |
|--------|--------|
| Screens Delivered | 49 screens |
| Design System Coverage | 100% |
| Responsive Breakpoints | 3 (Desktop, Tablet, Mobile) |
| Cross-Browser Support | 4 browsers |
| Navigation Working | 100% of links |
| Interactive Components | All functional |
| Stakeholder Approval | Sign-off on each milestone |

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-26 | Claude | Initial subagent specifications |
