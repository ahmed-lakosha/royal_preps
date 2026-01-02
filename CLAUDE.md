# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Royal Preps** - Medical exam preparation platform targeting UK medical students/doctors (MRCP, PLAB, MRCGP, UKMLA) and Egyptian medical professionals.

## Project Structure

```
royal_preps/
├── rad/
│   ├── researches/       # Competitive analysis, market research
│   ├── data/             # Excel files, PDFs (user stories, questions)
│   └── work-flow/        # Business specs, AI/ML requirements, monetization
└── CLAUDE.md
```

## Key Documentation

| Document | Location | Purpose |
|----------|----------|---------|
| PRD & User Stories | `rad/work-flow/prd_structure_and_user_stories_plan.md` | All epics, features, user stories |
| AI/ML Requirements | `rad/work-flow/medical_platform_ai_ml_implementation.md` | FSRS, IRT, RAG specs |
| Monetization | `rad/work-flow/medical_platform_monetization.md` | Pricing models, B2B strategy |
| Content/Licensing | `rad/work-flow/medical_content_creation_licensing.md` | Question creation, GDPR |
| Mobile Strategy | `rad/work-flow/mobile_strategy_react_native_vs_flutter.md` | Flutter recommendation |
| Platform Comparison | `rad/researches/2025-12-19_platform-comparison-medical-exam-prep-nextjs-django-odoo.md` | Django selection rationale |
| Competitive Analysis | `rad/researches/2025-12-19_medical-exam-platforms-competitive-analysis.md` | PassMedicine, Pastest, BMJ |
| Egypt Launch Strategy | `rad/researches/2025-12-19_egypt-medical-exam-platform-marketing-launch-strategy.md` | Egypt market entry |

## Business Context

- **Quotation-based sales** - No public pricing, salesperson-driven
- **Material-based subscriptions** - Per material + duration
- **User roles**: Visitor, Subscriber, Researcher, Salesperson, Admin
- **Question bank**: 3,000-7,000+ questions
- **Markets**: UK (GBP), Egypt (EGP localized)

## Development Rules

- **No inline scripts** - Create separate .js files
- **No inline styles** - Create separate .scss files
- **GitHub CLI** - Use `gh` commands for GitHub operations
- **No auto-push** - Only push when explicitly requested
- **Odoo core** - Never modify files in `@odoo\` directory
- **No DevOps tasks** - Keep all project work in the project folder
- **Notifications** - Use ntfy to notify after task completion or when user action needed
