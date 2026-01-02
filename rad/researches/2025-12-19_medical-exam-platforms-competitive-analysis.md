# Medical Exam Preparation Platforms - Comprehensive Competitive Analysis

## Metadata
- **Date**: December 19, 2025
- **Research ID**: MED-EXAM-2025-001
- **Domain**: Medical Education Technology / EdTech
- **Status**: Complete
- **Confidence**: High
- **Geographic Focus**: UK Medical Exams (MRCP, PLAB, MRCGP)

---

## Executive Summary

This comprehensive analysis examines three leading UK medical exam preparation platforms: **PassMedicine**, **Pastest**, and **BMJ OnExamination**. The research reveals a mature market with differentiated positioning: PassMedicine offers exceptional value with budget-friendly pricing and innovative spaced repetition; Pastest leads in content volume and premium features including AI tutoring; BMJ OnExamination leverages its medical publishing heritage for evidence-based content with strong peer benchmarking. Key findings indicate that successful platforms require extensive question banks (3,000-7,000+ questions), multiple study modes, mobile apps with offline access, performance analytics, and adaptive learning algorithms. The recommended technical stack for a competitive new platform includes modern web frameworks, PostgreSQL databases, Redis caching, and AI/ML integration for personalized learning.

---

## Table of Contents

1. [Platform Overview](#1-platform-overview)
2. [Core Features - Question Bank](#2-core-features---question-bank)
3. [Learning & Study Features](#3-learning--study-features)
4. [User Experience](#4-user-experience)
5. [Social & Collaborative Features](#5-social--collaborative-features)
6. [Technical Features](#6-technical-features)
7. [Unique Selling Points](#7-unique-selling-points)
8. [Feature Comparison Matrix](#8-feature-comparison-matrix)
9. [Recommended Features for New Platform](#9-recommended-features-for-new-platform)
10. [Technical Implementation Specifications](#10-technical-implementation-specifications)
11. [Sources and References](#11-sources-and-references)

---

## 1. Platform Overview

### 1.1 PassMedicine

#### Company Background
- **Founded**: 2014
- **Founder**: Jon Arnold (Founder & Managing Director)
- **Headquarters**: 71-75 Shelton Street, Covent Garden, London, WC2H 9JQ
- **Funding Status**: Unfunded (bootstrapped)
- **Years Operating**: 15+ years of medical revision resources

#### Target Audience
- Medical students (Years 1-5)
- Junior doctors preparing for postgraduate exams
- International Medical Graduates (IMGs)
- GP trainees

#### Supported Medical Exams
| Exam | Question Count | Features |
|------|---------------|----------|
| MRCP Part 1 | 5,100+ SBAs | 3 mock exams, 2 textbooks |
| MRCP Part 2 Written | 2,800+ SBAs | Image-based questions |
| MRCGP AKT | 4,500+ questions | 2025 curriculum aligned |
| PLAB Part 1 | 5,000+ questions | Gold-standard mock exam |
| PLAB Part 2 | Virtual patients | AI-powered history taking |
| Medical Finals/UKMLA | 11,000+ SBAs | OSCE & Prescribing Skills |
| MSRA | 3,000+ clinical + 300 dilemma | 2026 aligned |
| DRCOG | 1,000+ SBAs | - |
| USMLE Step 1 | 3,000+ SBAs | Flashcards included |
| UCAT | 3,000+ questions | 3 mock exams |
| Medical Student Years 1-3 | 4,700+ SBAs | ANKI-style tutor |

#### Pricing Models
| Duration | Price (GBP) | Per Month |
|----------|-------------|-----------|
| 4 months | ~£35 | ~£8.75 |
| 6 months | ~£45 | ~£7.50 |

**Value Proposition**: "Unbeatable price-to-content ratio" - significantly cheaper than competitors while maintaining quality.

#### User Base
- Serves UK medical students and doctors
- Growing international user base
- Partnered with NHS trusts for institutional access

---

### 1.2 Pastest

#### Company Background
- **Founded**: 1972 (50+ years in operation)
- **Founders**: Freydis and Nigel Campbell
- **Current Leadership**: Hugh Campbell (Chairman), Ross Duncan (CEO)
- **Headquarters**: No. 3 Booths Park, Knutsford, Cheshire, WA16 8GS
- **Annual Revenue**: ~$7.9 million (2025)
- **Employees**: 11-50

#### Historical Milestones
- 1972: Founded from kitchen of founders' home
- 1974: First UK medical revision book with explanations (MRCP Part 1 Practice Papers)
- 2005: Launched MRCP Part 1 online question bank
- 2014: Leadership transition to second generation
- 2022: Celebrated 50th anniversary
- 2023: Sold final physical book (now fully digital)

#### Target Audience
- Medical students and undergraduates
- Postgraduate medical trainees
- International Medical Graduates
- Specialty trainees across 22 medical/dental exams
- Users in 190 countries

#### Supported Medical Exams
| Exam Category | Specific Exams |
|---------------|----------------|
| Medical School | UCAT, UKMLA |
| MRCP | Part 1, Part 2, PACES |
| Surgery | MRCS Parts A & B |
| Paediatrics | MRCPCH (FOP/TAS, AKP, Clinical) |
| General Practice | MRCGP AKT |
| Other | PLAB 1, MSRA, FRCA Primary, Dentistry (MFDS, LDS, MJDF) |
| Language | OET, IELTS |

#### Pricing Models (MRCP Part 1 Example)
| Duration | Price (GBP) | Value |
|----------|-------------|-------|
| 3 months | £99.99 | For crammers |
| 6 months | £144.99 | For strivers |
| 12 months | £179.99 | Best value |
| 48 hours | Free | Trial |
| MRCP Membership (5 years) | £459.99 | Full catalogue access |

**Discounts**: Up to 30% off during Black Friday; Student Beans offers 3 months free with 12-month subscription.

#### User Base
- 300,000+ medical professionals globally
- 190 countries
- 70% pass rate for Pastest users vs 53% overall (MRCP Part 1 2023)

---

### 1.3 BMJ OnExamination

#### Company Background
- **Parent Company**: BMJ Publishing Group Limited
- **Company Registration**: 03102371 (England and Wales)
- **Headquarters**: BMA House, Tavistock Square, London, WC1H 9JR
- **Established Online**: Since 2011 (onexamination.com tracked since April 2011)
- **Heritage**: Part of BMJ Group, publishers of the British Medical Journal

#### Target Audience
- Medical students
- Core and specialist trainees
- GPs
- Doctors pursuing consultant positions
- International medical graduates

#### Supported Medical Exams
BMJ OnExamination offers 40+ examination preparation resources:

| Category | Exams |
|----------|-------|
| General Medicine | MRCP Part 1 & 2, MRCEM, SCE (multiple specialties) |
| Surgery | FRCS General Surgery, FRCS Trauma & Orthopaedic, MRCS Parts A |
| Anaesthesia/ICU | FRCA Primary & Final, FFICM |
| Paediatrics | MRCPCH (AKP, FOP, TAS) |
| O&G | MRCOG Part 1 & 2 |
| Psychiatry | MRCPsych Paper A & B |
| General Practice | MRCGP AKT |
| Other | PLAB, PSA, SJT, MSRA, MLA, DCH, DRCOG |

#### Pricing Models (MRCP Part 1)
| Duration | Price (GBP) |
|----------|-------------|
| 1 month | £49.99 |
| 3 months | £69.99 |
| 6 months | £99.99 |
| 12 months | £159.99 |

**Note**: 12-month plan is up to 50% cheaper per month than 1-month plan.

#### User Base
- 210,000+ medical professionals assisted
- 8,000+ questions answered per hour globally
- Strong institutional presence (NHS trusts, universities)

---

## 2. Core Features - Question Bank

### 2.1 Question Types Comparison

| Question Type | PassMedicine | Pastest | BMJ OnExamination |
|---------------|--------------|---------|-------------------|
| Single Best Answer (SBA) | Yes | Yes | Yes |
| Extended Matching Questions (EMQ) | Yes | Yes | Yes |
| Best of Five (BOF) | Yes | Yes | Yes |
| Multiple Best Answer (MBA) | Limited | Yes | Yes |
| Free Text Matching (FTM) | No | Yes (AKT) | No |
| Image-based Questions | Yes | Yes | Yes |
| Video-based Questions | No | Yes | Limited |

### 2.2 Question Bank Size by Exam

| Exam | PassMedicine | Pastest | BMJ OnExamination |
|------|--------------|---------|-------------------|
| MRCP Part 1 | 5,100+ | 5,400+ | 3,190 |
| MRCP Part 2 | 2,800+ | 5,000+ | 1,850+ |
| MRCGP AKT | 4,500+ | 3,400+ | 2,500+ (est.) |
| PLAB Part 1 | 5,000+ | Available | Available |
| Total Questions | ~35,000+ | ~50,000+ | ~30,000+ |

### 2.3 Question Categorization System

#### PassMedicine
- Organized by medical specialty/topic
- Mapped to exam syllabuses
- Tagged by difficulty level
- Flagging capability for user-created categories
- Key points extraction for revision

#### Pastest
- 600+ clinical topics (MRCP Part 1)
- 500+ topics (MRCP Part 2)
- 700+ topics (MRCGP AKT)
- Specialty-based filtering
- Question type filtering
- Difficulty filtering
- Keyword search
- Image-based filtering

#### BMJ OnExamination
- Curriculum-aligned categorization (Royal College of Physicians)
- Topic-based filtering
- Difficulty levels
- Question type filtering
- Keyword search
- "High Impact" ranking by clinical importance

### 2.4 Answer Explanations Format

#### PassMedicine
- Detailed teaching notes accompanying each question
- Notes build to form a reference library
- Evidence-based (national guidelines)
- Links to additional study resources
- Key points summary for quick review

#### Pastest
- Comprehensive explanations
- Expanded explanations (topic-wide, not just question-specific)
- References to clinical guidelines
- 3D interactive imagery in textbook
- Video explanations (bite-sized format)
- Podcast explanations available

#### BMJ OnExamination
- Comprehensive explanations linked to BMJ BestPractice
- Evidence-based content
- Key learning points summary
- Peer-reviewed content
- Updated to latest medical guidelines

### 2.5 References and Citations

| Platform | Citation Style | Sources |
|----------|---------------|---------|
| PassMedicine | National guidelines, evidence-based | NICE, BNF, specialty guidelines |
| Pastest | Academic and clinical | Royal Colleges, journals, guidelines |
| BMJ OnExamination | BMJ BestPractice integration | BMJ resources, clinical guidelines |

### 2.6 Image/Media Support

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|--------------|---------|-------------------|
| Clinical Images | Yes | Yes | Yes |
| Radiology (X-ray, CT, MRI) | Yes | Yes | Yes |
| ECGs | Yes | Yes | Yes |
| Dermatology Photos | Yes | Yes | Yes |
| Histopathology | Yes | Yes | Yes |
| 3D Interactive Models | No | Yes | No |
| Video Content | Limited | Extensive | Limited |
| Podcasts | No | Yes | No |

### 2.7 Question Difficulty Levels

#### PassMedicine
- Implicit difficulty through performance tracking
- Knowledge Tutor prioritizes by relevance/difficulty
- Performance histogram for comparison

#### Pastest
- Explicit difficulty levels
- Familiarity tracking
- iSAAC AI adapts to user level
- Past paper difficulty matching

#### BMJ OnExamination
- Explicit difficulty levels
- "Work Smart" feature adjusts based on performance
- Peer difficulty comparison
- "High Impact" question ranking

### 2.8 Spaced Repetition / Adaptive Learning

| Platform | Feature Name | Algorithm |
|----------|--------------|-----------|
| PassMedicine | Knowledge Tutor | ANKI-style spaced repetition, priority-based |
| Pastest | iSAAC | AI-driven content adaptation |
| BMJ OnExamination | Work Smart | Performance-based question selection |

---

## 3. Learning & Study Features

### 3.1 Study Modes

| Mode | PassMedicine | Pastest | BMJ OnExamination |
|------|--------------|---------|-------------------|
| Revision/Tutor Mode | Yes | Yes | Yes |
| Timed Test Mode | Yes | Yes | Yes |
| Exam Simulation Mode | Yes (Mock Exams) | Yes (Past Papers) | Yes (Mock Tests) |
| Untimed Practice | Yes | Yes | Yes |
| Random Questions | Yes | Yes | Yes |
| Topic-Focused | Yes | Yes | Yes |
| Flashcard Mode | No (Knowledge Tutor instead) | Yes | Yes |

### 3.2 Custom Test Creation

#### PassMedicine
- Select by topic/specialty
- Choose question count
- Timed or untimed options
- Filter by previously answered/flagged
- Create personalized revision sessions

#### Pastest
- Up to 100 questions per session
- Filter by: specialty, question type, difficulty, familiarity, images, keywords
- Create from incorrect answers
- Create from flagged questions
- "Continue previous session" function

#### BMJ OnExamination
- Custom difficulty selection
- Topic filtering
- Question type selection
- Review challenging material
- Recently: Simplified to 20-question sets (controversial update)

### 3.3 Progress Tracking and Analytics

#### PassMedicine
- Performance comparison vs other candidates
- Daily-updated histogram showing score distribution
- Readiness assessment for exam
- Topic-by-topic performance breakdown
- Question completion tracking

#### Pastest
- Easy-to-digest performance overview
- Progress synced across devices
- Specialty performance breakdown
- Trend analysis over time
- Mock exam scoring with percentile ranking

#### BMJ OnExamination
- Detailed performance graphs
- Peer benchmarking
- Pass probability indicator
- Strength and weakness identification
- Personal performance feedback

### 3.4 Performance Reports and Statistics

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|--------------|---------|-------------------|
| Overall Score | Yes | Yes | Yes |
| Topic Breakdown | Yes | Yes | Yes |
| Percentile Rank | Yes (histogram) | Yes | Yes |
| Trend Over Time | Yes | Yes | Yes |
| Comparison to Peers | Yes | Yes | Yes |
| Pass Prediction | Implicit | Explicit | Explicit |
| Exportable Reports | Limited | Yes | Yes |

### 3.5 Weak Area Identification

#### PassMedicine
- Automatic identification through performance tracking
- Knowledge Tutor focuses on weak areas
- Visual dashboard showing topic performance

#### Pastest
- iSAAC AI identifies and targets weak areas
- Expanded explanations for common weak topics
- Performance analytics highlight struggling areas
- Personalized study material adjustment

#### BMJ OnExamination
- Automatic weak area detection
- Reporting metrics highlight struggling areas
- "Revisit incorrect questions" feature
- Focus revision recommendations

### 3.6 Revision Scheduling

| Platform | Feature |
|----------|---------|
| PassMedicine | Knowledge Tutor auto-schedules based on spaced repetition |
| Pastest | Manual planning with progress tracking |
| BMJ OnExamination | Daily Question Service (personalized daily notifications) |

### 3.7 Flashcards / Notes Features

#### PassMedicine
- Knowledge Tutor (flashcard-style facts)
- ANKI-style algorithm
- Thousands of flashcard-style facts (USMLE)
- User can add personal notes to questions
- Key points extraction

#### Pastest
- Dedicated flashcard feature
- Integrated into textbook
- Searchable flashcard library
- Specialty-organized

#### BMJ OnExamination
- Personalized flashcards
- Key learning points as flashcards
- Bookmark questions for review

### 3.8 Video Content / Lectures

| Content Type | PassMedicine | Pastest | BMJ OnExamination |
|--------------|--------------|---------|-------------------|
| Teaching Videos | No | Yes (extensive) | Limited |
| Bite-sized Videos | No | Yes (integrated) | No |
| Podcasts | No | Yes | No |
| PACES Videos | No | 130+ gold-standard | AI PACES tool |
| Video Playback Speed | N/A | 2x available | N/A |

#### Pastest Video Topics (MRCP Part 1)
- Neurology
- Haematology
- Clinical Pharmacology
- Infectious Diseases
- Nephrology
- Additional topics being added

---

## 4. User Experience

### 4.1 User Dashboard Design

#### PassMedicine
- Clean, functional interface
- Question bank central focus
- Performance histogram prominently displayed
- Quick access to Knowledge Tutor
- Topic navigation sidebar
- Mobile-optimized views

#### Pastest
- Modern, feature-rich dashboard
- "Continue previous session" prominent
- Quick access to past papers
- Video/podcast library accessible
- Progress overview visible
- Multiple resource types organized

#### BMJ OnExamination
- Performance-focused dashboard
- Peer comparison visible
- Quick question access
- Daily question notifications
- Clean mobile interface
- Gamification elements (leaderboard)

### 4.2 Mobile App Availability

| Platform | iOS | Android | PWA |
|----------|-----|---------|-----|
| PassMedicine | Yes (installable from website) | Yes (installable from website) | Yes |
| Pastest | Yes (App Store) | Yes (Google Play) | No |
| BMJ OnExamination | Yes (App Store) | Yes (Google Play) | No |

#### PassMedicine Mobile App
- Installed directly from website (not app stores)
- Optimized UI for smaller screens
- Offline access to questions
- Offline Knowledge Tutor access
- Multi-device sync
- No login timeout
- Rating: N/A (not in app stores)

#### Pastest Mobile App
- Native app (Spring 2023 release)
- Full question bank access
- Download videos/podcasts for offline
- Offline question practice
- Sync with desktop
- Rating: 3.06/5 (480 ratings)
- Size: ~53MB

**Reported Issues**:
- Question log accuracy problems
- Offline sync issues (historically)
- Interface described as "clunky" by some

#### BMJ OnExamination Mobile App
- Native iOS and Android apps
- Up to 100 questions offline
- Cloud synchronization
- Landscape mode support
- Rating: Mixed (functionality issues reported)

**Reported Issues**:
- App freezing on some Android versions
- Tagging/filtering not working properly
- November 2024 update removed category selection

### 4.3 Offline Access Capabilities

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|--------------|---------|-------------------|
| Offline Questions | Yes | Yes | Yes (100 max) |
| Offline Textbook | Yes | Yes | No |
| Offline Videos | No | Yes | No |
| Offline Podcasts | No | Yes | No |
| Auto-Sync | Yes | Yes | Yes |

### 4.4 Bookmark/Flagging Questions

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|--------------|---------|-------------------|
| Flag Questions | Yes | Yes | Yes |
| Add Personal Notes | Yes | Yes | Limited |
| Create Custom Lists | Limited | Yes | Yes |
| Filter Flagged | Yes | Yes | Reported issues |
| Multiple Flag Categories | No | Yes | No |

### 4.5 Search and Filter Functionality

#### PassMedicine
- Topic/specialty search
- Filter by answered/unanswered
- Filter by flagged
- Keyword search in questions

#### Pastest
- Comprehensive filters:
  - Specialty
  - Question type
  - Difficulty
  - Familiarity
  - Image-based
  - Keyword search
- Session customization up to 100 questions

#### BMJ OnExamination
- Topic filtering
- Difficulty filtering
- Question type filtering
- Keyword search
- **Note**: November 2024 update simplified/removed some filters (user complaints)

### 4.6 User Interface Quality Assessment

| Criteria | PassMedicine | Pastest | BMJ OnExamination |
|----------|--------------|---------|-------------------|
| Overall Design | Clean, functional | Modern, feature-rich | Professional, clean |
| Ease of Use | High | Medium | High |
| Learning Curve | Low | Medium | Low |
| Mobile Experience | Good | Mixed reviews | Mixed reviews |
| Accessibility | Standard | Standard | Standard |
| Dark Mode | No | Requested by users | No |
| Load Speed | Fast | Generally good | Variable |

---

## 5. Social & Collaborative Features

### 5.1 Discussion Forums

| Platform | Forum Available | Features |
|----------|-----------------|----------|
| PassMedicine | No dedicated forum | N/A |
| Pastest | WhatsApp community | Direct support |
| BMJ OnExamination | No dedicated forum | N/A |

### 5.2 Peer Comparisons

#### PassMedicine
- Daily-updated histogram showing score distribution
- Compare to "other candidates about to sit exam"
- Percentile positioning

#### Pastest
- Mock exam percentile ranking
- Performance benchmarking
- 70% pass rate claim vs 53% overall

#### BMJ OnExamination
- Detailed peer comparison graphs
- "Benchmark against your peers"
- Daily leaderboard
- Friend competitions

### 5.3 Study Groups

| Platform | Study Groups | Implementation |
|----------|--------------|----------------|
| PassMedicine | No | N/A |
| Pastest | No formal feature | WhatsApp community |
| BMJ OnExamination | Yes | Compete with friends via username |

#### BMJ OnExamination Group Features
- Play under username
- Join friends for 10-question sessions
- Daily leaderboard
- Simple PIN for group sessions

### 5.4 Tutor/Mentor Access

| Platform | Tutor Access | Features |
|----------|--------------|----------|
| PassMedicine | No live tutors | AI Knowledge Tutor |
| Pastest | AI Tutor (Beta) | On-demand hints, instant answers |
| BMJ OnExamination | No live tutors | BMJ BestPractice integration |

#### Pastest AI Tutor Features
- Exclusively for MRCP Part 1
- On-demand hints
- Instant answers
- Re-explain in simpler terms
- Real-time insights
- 6,001 questions asked in first month of launch

### 5.5 Community Features Summary

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|--------------|---------|-------------------|
| User Forums | No | No | No |
| Peer Comparison | Yes | Yes | Yes |
| Study Groups | No | No | Yes (limited) |
| Leaderboards | No | No | Yes |
| Social Login | No | No | No |
| Share Progress | No | No | No |
| Discussion Threads | No | No | No |

---

## 6. Technical Features

### 6.1 Authentication Systems

| Platform | Authentication Methods |
|----------|----------------------|
| PassMedicine | Email/password, session-based |
| Pastest | Email/password, app-based |
| BMJ OnExamination | Email/password, NHS OpenAthens (institutional) |

#### Institutional Access
- **PassMedicine**: NHS trust codes (4-month access typical)
- **Pastest**: Institutional subscriptions available
- **BMJ OnExamination**: Institutional voucher system, NHS OpenAthens integration

### 6.2 Payment Integration

| Platform | Payment Methods |
|----------|-----------------|
| PassMedicine | Credit/debit cards (likely Stripe) |
| Pastest | Credit/debit cards, likely Stripe |
| BMJ OnExamination | Credit/debit cards, App Store/Google Play in-app purchases |

### 6.3 API Capabilities

Based on research, none of the platforms offer public APIs for third-party integration. All are closed ecosystems.

### 6.4 Integration with Other Platforms

| Platform | Integrations |
|----------|--------------|
| PassMedicine | None identified |
| Pastest | WhatsApp (community), social media |
| BMJ OnExamination | BMJ BestPractice, SimConverse (AI PACES) |

### 6.5 Content Updates Frequency

| Platform | Update Frequency |
|----------|------------------|
| PassMedicine | Continuous (aligned with guidelines) |
| Pastest | Regular (aligned with exam changes, RCP feedback) |
| BMJ OnExamination | Regular (curriculum-aligned updates) |

---

## 7. Unique Selling Points

### 7.1 PassMedicine

#### Competitive Advantages
1. **Price Leadership**: Significantly cheaper than competitors (~£35/4 months vs £100+)
2. **Knowledge Tutor**: Unique spaced repetition system (ANKI-style)
3. **Value Ratio**: "Unbeatable price-to-content ratio"
4. **Question Similarity**: Users report questions "more similar to actual exam"
5. **Comprehensive Textbooks**: Two textbooks included (high-yield + extended)
6. **15+ Years Experience**: Established reputation

#### Known Limitations
- Fewer features than Pastest
- No video/podcast content
- Some questions reported outdated
- App not in official app stores
- No AI tutor feature
- Limited community features

#### User Complaints (Trustpilot - 3.2/5, 17 reviews)
- DRCOG content gaps reported
- UCAT questions easier than actual exam
- Question writing/editorial process issues
- Website downtime incidents

---

### 7.2 Pastest

#### Competitive Advantages
1. **Largest Question Bank**: 5,400+ MRCP Part 1 questions
2. **50+ Years Heritage**: Established 1972, trusted brand
3. **Multi-Media Learning**: Videos, podcasts, 3D imagery
4. **AI Tutor (Beta)**: Cutting-edge personalized assistance
5. **iSAAC Algorithm**: AI-driven adaptive learning
6. **Past Papers**: Tailored to recent exam themes
7. **PACES Videos**: 130+ gold-standard examination videos
8. **Higher Pass Rates**: 70% vs 53% overall (claimed)
9. **Comprehensive Coverage**: 600+ clinical topics

#### Known Limitations
- Higher price point
- App has mixed reviews (syncing issues)
- No dark mode
- Navigation between questions can be cumbersome
- Subscription access issues reported

#### User Complaints (Trustpilot - Mixed, 5,139+ reviews)
- App synchronization problems
- Technical issues with videos on mobile
- Navigation difficulties
- Subscription activation issues
- Podcast functionality issues in app

---

### 7.3 BMJ OnExamination

#### Competitive Advantages
1. **BMJ Heritage**: Part of British Medical Journal group
2. **Evidence-Based**: Linked to BMJ BestPractice
3. **Peer Benchmarking**: Detailed comparison features
4. **AI PACES Tool**: First AI-driven OSCE revision tool
5. **Daily Question Service**: Personalized daily notifications
6. **Gamification**: Leaderboards and friend competitions
7. **Expert Authors**: Past examiners, field specialists
8. **210,000+ Users**: Established user base
9. **Curriculum-Aligned**: Royal College of Physicians alignment

#### Known Limitations
- Smaller question bank than competitors
- November 2024 update removed popular features
- App stability issues on some devices
- Higher price per question
- Limited video content

#### User Complaints
- November 2024 app update removed category filtering
- App freezing issues (Android)
- Tagging features not working
- Content currency concerns (one university discontinued subscription)
- Some question inaccuracies reported

---

## 8. Feature Comparison Matrix

### 8.1 Question Bank Features

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|:------------:|:-------:|:-----------------:|
| MRCP Part 1 Questions | 5,100+ | 5,400+ | 3,190 |
| MRCP Part 2 Questions | 2,800+ | 5,000+ | 1,850+ |
| MRCGP AKT Questions | 4,500+ | 3,400+ | 2,500+ |
| PLAB Questions | 5,000+ | Available | Available |
| SBA Format | Yes | Yes | Yes |
| EMQ Format | Yes | Yes | Yes |
| Image-based Questions | Yes | Yes | Yes |
| Video Questions | No | Yes | Limited |
| Detailed Explanations | Yes | Yes | Yes |
| References/Citations | Yes | Yes | Yes (BMJ BestPractice) |

### 8.2 Learning Features

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|:------------:|:-------:|:-----------------:|
| Spaced Repetition | Yes (Knowledge Tutor) | Limited | Yes (Work Smart) |
| AI-Adaptive Learning | No | Yes (iSAAC) | Yes |
| AI Tutor | No | Yes (Beta) | No |
| Mock Exams | 3 per exam | 34 past papers | Yes |
| Video Lectures | No | Yes (extensive) | Limited |
| Podcasts | No | Yes | No |
| Flashcards | ANKI-style | Yes | Yes |
| Textbook Included | 2 textbooks | Yes (searchable) | No |
| 3D Interactive Models | No | Yes | No |
| OSCE/Clinical Videos | No | 130+ | AI PACES |

### 8.3 User Experience Features

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|:------------:|:-------:|:-----------------:|
| iOS App | Yes (PWA) | Yes (Native) | Yes (Native) |
| Android App | Yes (PWA) | Yes (Native) | Yes (Native) |
| Offline Access | Yes | Yes | Yes (100 questions) |
| Cross-Device Sync | Yes | Yes | Yes |
| Dark Mode | No | No | No |
| Bookmark Questions | Yes | Yes | Yes |
| Personal Notes | Yes | Yes | Limited |
| Search Functionality | Yes | Comprehensive | Yes |
| Filter Options | Basic | Extensive | Recently reduced |

### 8.4 Social Features

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|:------------:|:-------:|:-----------------:|
| Peer Comparison | Yes | Yes | Yes |
| Leaderboards | No | No | Yes |
| Study Groups | No | No | Limited |
| Discussion Forum | No | No | No |
| Social Sharing | No | No | No |

### 8.5 Technical Features

| Feature | PassMedicine | Pastest | BMJ OnExamination |
|---------|:------------:|:-------:|:-----------------:|
| Institutional Access | Yes (NHS codes) | Yes | Yes (OpenAthens) |
| Free Trial | No | 48 hours | 10 free questions/day |
| Multiple Payment Options | Yes | Yes | Yes + In-App |
| API Access | No | No | No |
| Third-Party Integrations | No | Limited | BMJ BestPractice |

### 8.6 Pricing Comparison (MRCP Part 1)

| Duration | PassMedicine | Pastest | BMJ OnExamination |
|----------|:------------:|:-------:|:-----------------:|
| 1 month | N/A | N/A | £49.99 |
| 3 months | N/A | £99.99 | £69.99 |
| 4 months | ~£35 | N/A | £79.99 |
| 6 months | ~£45 | £144.99 | £99.99 |
| 12 months | N/A | £179.99 | £159.99 |
| Free Trial | No | 48 hours | 10 questions/day |

### 8.7 Overall Ratings Summary

| Metric | PassMedicine | Pastest | BMJ OnExamination |
|--------|:------------:|:-------:|:-----------------:|
| Trustpilot Rating | 3.2/5 (17 reviews) | Mixed (5,139+ reviews) | 4.3-4.8/5 |
| App Store Rating | N/A | 3.06/5 | Mixed |
| Price Value | Excellent | Good | Good |
| Content Volume | Very Good | Excellent | Good |
| Feature Richness | Good | Excellent | Good |
| Ease of Use | Excellent | Good | Good |

---

## 9. Recommended Features for New Platform

### 9.1 Essential Features (MVP Requirements)

#### Question Bank Core
1. **Minimum 3,000+ questions per major exam** (MRCP, MRCGP, PLAB)
2. **Multiple question formats**: SBA, EMQ, BOF, MBA
3. **Comprehensive explanations** with evidence-based references
4. **Image support**: Clinical images, radiology, ECGs, dermatology
5. **Curriculum alignment**: Map to Royal College syllabuses
6. **Regular content updates**: Align with guideline changes

#### Study Modes
1. **Revision/Tutor Mode**: Untimed, with immediate feedback
2. **Timed Test Mode**: Configurable time limits
3. **Mock Exam Mode**: Full exam simulation
4. **Custom Test Builder**: Filter by topic, difficulty, question type
5. **Review Mode**: Revisit incorrect/flagged questions

#### Progress Tracking
1. **Performance analytics dashboard**
2. **Topic-by-topic breakdown**
3. **Trend analysis over time**
4. **Peer comparison/benchmarking**
5. **Pass probability indicator**

#### Mobile Experience
1. **Native iOS and Android apps**
2. **Offline access** (minimum 100 questions)
3. **Cross-device synchronization**
4. **Responsive web design**
5. **Push notifications** for daily questions

#### User Features
1. **Bookmark/flag questions**
2. **Personal notes on questions**
3. **Search and filter functionality**
4. **Account management**
5. **Subscription management**

### 9.2 Nice-to-Have Features (Phase 2+)

#### Advanced Learning
1. **Spaced Repetition Algorithm** (like Knowledge Tutor)
2. **AI-Adaptive Learning** (like iSAAC)
3. **AI Tutor/Chat** (like Pastest AI Tutor)
4. **Flashcard System**
5. **Integrated Textbook** (searchable, linked to questions)
6. **Video Lectures** (bite-sized, specialty-focused)
7. **Podcasts** for audio learning
8. **3D Interactive Models** for anatomy/procedures

#### Social/Community
1. **Leaderboards and gamification**
2. **Study group functionality**
3. **Friend competitions**
4. **Discussion forums per question**
5. **Peer question explanations**
6. **Social sharing of achievements**

#### Technical Enhancements
1. **Dark mode**
2. **Multiple language support**
3. **Accessibility features** (screen reader, high contrast)
4. **Advanced analytics export**
5. **Calendar integration for study planning**
6. **Institutional admin dashboard**
7. **API for third-party integrations**

#### Content Enhancements
1. **Clinical case videos** (OSCE/PACES)
2. **AI-powered virtual patient interactions**
3. **Prescribing skills module**
4. **Communication skills training**
5. **Ethical scenarios module**

### 9.3 Feature Priority Matrix

| Feature | Impact | Effort | Priority |
|---------|:------:|:------:|:--------:|
| Question Bank (3000+) | High | High | P0 |
| Mobile Apps | High | High | P0 |
| Progress Tracking | High | Medium | P0 |
| Mock Exams | High | Medium | P0 |
| Offline Access | High | Medium | P1 |
| Spaced Repetition | High | Medium | P1 |
| Peer Benchmarking | Medium | Low | P1 |
| AI Tutor | High | High | P2 |
| Video Content | Medium | High | P2 |
| Flashcards | Medium | Low | P2 |
| Study Groups | Low | Medium | P3 |
| Discussion Forums | Low | Medium | P3 |

---

## 10. Technical Implementation Specifications

### 10.1 Recommended Technology Stack

#### Frontend
```
- Framework: React.js or Next.js (SSR for SEO)
- State Management: Redux Toolkit or Zustand
- UI Components: Tailwind CSS + Headless UI or Material-UI
- Charts/Analytics: Chart.js or D3.js
- Mobile: React Native (cross-platform iOS/Android)
- PWA Support: Service Workers for offline capability
```

#### Backend
```
- Framework: Node.js with Express/Fastify OR Python with Django/FastAPI
- API: RESTful with GraphQL consideration for complex queries
- Authentication: JWT + OAuth 2.0 (social login optional)
- Real-time: WebSockets for live features (leaderboards, group study)
```

#### Database Architecture
```
Primary Database: PostgreSQL 15+
- Relational data: Users, subscriptions, questions, answers
- JSONB for flexible question metadata
- Full-text search for question/textbook search

Cache Layer: Redis
- Session management
- Spaced repetition queue
- Leaderboard data
- API rate limiting

Search: Elasticsearch (optional)
- Advanced question search
- Textbook full-text search
- Analytics queries

File Storage: AWS S3 / Cloudflare R2
- Question images
- Video content
- User uploads
```

#### Infrastructure
```
Cloud Provider: AWS / GCP / Azure
- Kubernetes (EKS/GKE) for container orchestration
- CDN: CloudFront / Cloudflare for static assets
- Load Balancer: Application Load Balancer
- Auto-scaling for traffic spikes (exam periods)

CI/CD: GitHub Actions / GitLab CI
- Automated testing
- Staged deployments
- Database migrations
```

### 10.2 Database Schema (Core Entities)

```sql
-- Users and Authentication
CREATE TABLE users (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    email VARCHAR(255) UNIQUE NOT NULL,
    password_hash VARCHAR(255) NOT NULL,
    first_name VARCHAR(100),
    last_name VARCHAR(100),
    role VARCHAR(50) DEFAULT 'student', -- student, admin, author, institution
    institution_id UUID REFERENCES institutions(id),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    last_login TIMESTAMP,
    email_verified BOOLEAN DEFAULT FALSE,
    preferences JSONB DEFAULT '{}'
);

-- Subscriptions
CREATE TABLE subscriptions (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    exam_id UUID REFERENCES exams(id),
    plan_type VARCHAR(50), -- monthly, quarterly, annual
    status VARCHAR(50), -- active, expired, cancelled
    start_date TIMESTAMP NOT NULL,
    end_date TIMESTAMP NOT NULL,
    payment_provider VARCHAR(50), -- stripe, paypal
    payment_id VARCHAR(255),
    amount_paid DECIMAL(10,2),
    currency VARCHAR(3) DEFAULT 'GBP',
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Exams Catalog
CREATE TABLE exams (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    name VARCHAR(255) NOT NULL, -- 'MRCP Part 1'
    code VARCHAR(50) UNIQUE NOT NULL, -- 'mrcp-1'
    category VARCHAR(100), -- 'Postgraduate', 'Medical School'
    description TEXT,
    exam_body VARCHAR(255), -- 'Royal College of Physicians'
    pass_mark INTEGER,
    total_questions INTEGER,
    duration_minutes INTEGER,
    is_active BOOLEAN DEFAULT TRUE,
    syllabus_version VARCHAR(50),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Questions
CREATE TABLE questions (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    exam_id UUID REFERENCES exams(id),
    question_type VARCHAR(50) NOT NULL, -- 'SBA', 'EMQ', 'BOF', 'MBA'
    difficulty VARCHAR(20), -- 'easy', 'medium', 'hard'
    topic_id UUID REFERENCES topics(id),
    stem TEXT NOT NULL, -- The question text
    clinical_scenario TEXT, -- Extended clinical context
    options JSONB NOT NULL, -- Array of answer options
    correct_answer JSONB NOT NULL, -- Correct answer(s)
    explanation TEXT NOT NULL,
    key_learning_points JSONB, -- Array of key points
    references JSONB, -- Citations and sources
    images JSONB, -- Array of image URLs
    tags JSONB, -- Additional tags for filtering
    author_id UUID REFERENCES users(id),
    reviewer_id UUID REFERENCES users(id),
    status VARCHAR(50) DEFAULT 'draft', -- draft, review, published, archived
    version INTEGER DEFAULT 1,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    published_at TIMESTAMP
);

-- Topics/Categories
CREATE TABLE topics (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    exam_id UUID REFERENCES exams(id),
    parent_id UUID REFERENCES topics(id), -- For hierarchical topics
    name VARCHAR(255) NOT NULL,
    code VARCHAR(100),
    description TEXT,
    syllabus_reference VARCHAR(255),
    order_index INTEGER,
    is_active BOOLEAN DEFAULT TRUE
);

-- User Question Attempts
CREATE TABLE question_attempts (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    question_id UUID REFERENCES questions(id),
    session_id UUID REFERENCES study_sessions(id),
    selected_answer JSONB NOT NULL,
    is_correct BOOLEAN NOT NULL,
    time_spent_seconds INTEGER,
    confidence_level INTEGER, -- 1-5 self-reported confidence
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,

    INDEX idx_user_question (user_id, question_id),
    INDEX idx_session (session_id)
);

-- Study Sessions
CREATE TABLE study_sessions (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    exam_id UUID REFERENCES exams(id),
    session_type VARCHAR(50), -- 'revision', 'timed', 'mock'
    status VARCHAR(50) DEFAULT 'in_progress', -- in_progress, completed, abandoned
    total_questions INTEGER,
    questions_answered INTEGER DEFAULT 0,
    correct_answers INTEGER DEFAULT 0,
    time_limit_minutes INTEGER,
    time_spent_seconds INTEGER,
    filters_applied JSONB, -- Topic, difficulty, etc.
    question_ids JSONB, -- Ordered array of question IDs
    started_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    completed_at TIMESTAMP,
    score_percentage DECIMAL(5,2)
);

-- Mock Exams
CREATE TABLE mock_exams (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    exam_id UUID REFERENCES exams(id),
    name VARCHAR(255) NOT NULL,
    description TEXT,
    question_count INTEGER NOT NULL,
    time_limit_minutes INTEGER NOT NULL,
    question_distribution JSONB, -- Topic distribution
    is_active BOOLEAN DEFAULT TRUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Bookmarks/Flags
CREATE TABLE bookmarks (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    question_id UUID REFERENCES questions(id),
    category VARCHAR(100) DEFAULT 'general', -- 'review', 'difficult', 'important'
    notes TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,

    UNIQUE(user_id, question_id)
);

-- User Notes
CREATE TABLE user_notes (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    question_id UUID REFERENCES questions(id),
    content TEXT NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Spaced Repetition Queue
CREATE TABLE spaced_repetition_items (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    question_id UUID REFERENCES questions(id),
    ease_factor DECIMAL(4,2) DEFAULT 2.5, -- SM-2 algorithm
    interval_days INTEGER DEFAULT 1,
    repetitions INTEGER DEFAULT 0,
    next_review_date DATE,
    last_reviewed_at TIMESTAMP,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,

    UNIQUE(user_id, question_id)
);

-- Performance Analytics (Aggregated)
CREATE TABLE user_performance_daily (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID REFERENCES users(id),
    exam_id UUID REFERENCES exams(id),
    date DATE NOT NULL,
    questions_attempted INTEGER DEFAULT 0,
    questions_correct INTEGER DEFAULT 0,
    time_spent_seconds INTEGER DEFAULT 0,
    topics_studied JSONB, -- Topic breakdown

    UNIQUE(user_id, exam_id, date)
);

-- Institutions
CREATE TABLE institutions (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    name VARCHAR(255) NOT NULL,
    type VARCHAR(100), -- 'nhs_trust', 'university', 'hospital'
    contact_email VARCHAR(255),
    subscription_type VARCHAR(50),
    max_users INTEGER,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Institutional Access Codes
CREATE TABLE access_codes (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    institution_id UUID REFERENCES institutions(id),
    code VARCHAR(50) UNIQUE NOT NULL,
    exam_id UUID REFERENCES exams(id),
    duration_days INTEGER NOT NULL,
    max_uses INTEGER,
    uses_count INTEGER DEFAULT 0,
    valid_from TIMESTAMP,
    valid_until TIMESTAMP,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### 10.3 API Structure (RESTful)

```yaml
# Authentication
POST   /api/v1/auth/register
POST   /api/v1/auth/login
POST   /api/v1/auth/logout
POST   /api/v1/auth/refresh-token
POST   /api/v1/auth/forgot-password
POST   /api/v1/auth/reset-password
GET    /api/v1/auth/verify-email/{token}

# Users
GET    /api/v1/users/me
PUT    /api/v1/users/me
PUT    /api/v1/users/me/preferences
GET    /api/v1/users/me/subscriptions
GET    /api/v1/users/me/performance

# Exams
GET    /api/v1/exams
GET    /api/v1/exams/{examId}
GET    /api/v1/exams/{examId}/topics
GET    /api/v1/exams/{examId}/mock-exams

# Questions
GET    /api/v1/exams/{examId}/questions
GET    /api/v1/questions/{questionId}
POST   /api/v1/questions/{questionId}/attempt
GET    /api/v1/questions/{questionId}/explanation

# Study Sessions
POST   /api/v1/sessions/create
GET    /api/v1/sessions/{sessionId}
PUT    /api/v1/sessions/{sessionId}
POST   /api/v1/sessions/{sessionId}/submit
GET    /api/v1/sessions/{sessionId}/results

# Mock Exams
POST   /api/v1/mock-exams/{mockId}/start
GET    /api/v1/mock-exams/{mockId}/session/{sessionId}
POST   /api/v1/mock-exams/{mockId}/session/{sessionId}/submit

# Bookmarks
GET    /api/v1/bookmarks
POST   /api/v1/bookmarks
DELETE /api/v1/bookmarks/{bookmarkId}

# Notes
GET    /api/v1/questions/{questionId}/notes
POST   /api/v1/questions/{questionId}/notes
PUT    /api/v1/notes/{noteId}
DELETE /api/v1/notes/{noteId}

# Analytics
GET    /api/v1/analytics/performance
GET    /api/v1/analytics/performance/topics
GET    /api/v1/analytics/performance/trends
GET    /api/v1/analytics/peer-comparison

# Spaced Repetition
GET    /api/v1/spaced-repetition/queue
POST   /api/v1/spaced-repetition/review

# Subscriptions
GET    /api/v1/subscriptions/plans
POST   /api/v1/subscriptions/checkout
POST   /api/v1/subscriptions/webhook (Stripe/PayPal)
POST   /api/v1/subscriptions/redeem-code

# Admin (Protected)
GET    /api/v1/admin/questions
POST   /api/v1/admin/questions
PUT    /api/v1/admin/questions/{questionId}
GET    /api/v1/admin/users
GET    /api/v1/admin/analytics
```

### 10.4 Spaced Repetition Algorithm (SM-2)

```python
# Implementation of SuperMemo SM-2 Algorithm
def calculate_next_review(quality: int, repetitions: int,
                          ease_factor: float, interval: int) -> tuple:
    """
    Calculate next review date using SM-2 algorithm.

    Args:
        quality: User's response quality (0-5)
            0 - Complete blackout
            1 - Incorrect; correct answer remembered
            2 - Incorrect; correct answer easy to recall
            3 - Correct with serious difficulty
            4 - Correct with hesitation
            5 - Perfect response
        repetitions: Number of times reviewed
        ease_factor: Current ease factor (starts at 2.5)
        interval: Current interval in days

    Returns:
        tuple: (new_repetitions, new_ease_factor, new_interval)
    """

    if quality < 3:
        # Failed - reset
        new_repetitions = 0
        new_interval = 1
    else:
        # Success
        if repetitions == 0:
            new_interval = 1
        elif repetitions == 1:
            new_interval = 6
        else:
            new_interval = round(interval * ease_factor)

        new_repetitions = repetitions + 1

    # Update ease factor
    new_ease_factor = ease_factor + (0.1 - (5 - quality) * (0.08 + (5 - quality) * 0.02))

    # Minimum ease factor
    if new_ease_factor < 1.3:
        new_ease_factor = 1.3

    return (new_repetitions, new_ease_factor, new_interval)
```

### 10.5 Performance Benchmarking Algorithm

```python
def calculate_percentile_rank(user_score: float, exam_id: str) -> int:
    """
    Calculate user's percentile rank compared to peers.

    Uses a pre-computed histogram or real-time calculation
    based on recent exam takers (e.g., last 30 days).
    """

    # Query recent scores for the exam
    recent_scores = db.query("""
        SELECT score_percentage
        FROM user_performance_daily
        WHERE exam_id = %s
        AND date >= NOW() - INTERVAL '30 days'
        ORDER BY score_percentage
    """, [exam_id])

    if not recent_scores:
        return 50  # Default to 50th percentile if no data

    # Count how many scores are below user's score
    below_count = sum(1 for score in recent_scores if score < user_score)

    # Calculate percentile
    percentile = (below_count / len(recent_scores)) * 100

    return round(percentile)
```

### 10.6 Payment Integration (Stripe)

```javascript
// Stripe Checkout Session Creation
const stripe = require('stripe')(process.env.STRIPE_SECRET_KEY);

async function createCheckoutSession(userId, planId, examId) {
  const plan = await getPlanDetails(planId);

  const session = await stripe.checkout.sessions.create({
    payment_method_types: ['card'],
    line_items: [{
      price_data: {
        currency: 'gbp',
        product_data: {
          name: `${plan.examName} - ${plan.duration} months`,
          description: plan.description,
        },
        unit_amount: plan.priceInPence, // e.g., 3500 for £35
      },
      quantity: 1,
    }],
    mode: 'payment',
    success_url: `${BASE_URL}/subscription/success?session_id={CHECKOUT_SESSION_ID}`,
    cancel_url: `${BASE_URL}/subscription/cancelled`,
    metadata: {
      userId: userId,
      planId: planId,
      examId: examId,
    },
    customer_email: await getUserEmail(userId),
  });

  return session;
}

// Webhook Handler
async function handleStripeWebhook(event) {
  switch (event.type) {
    case 'checkout.session.completed':
      const session = event.data.object;
      await activateSubscription(
        session.metadata.userId,
        session.metadata.planId,
        session.metadata.examId,
        session.id
      );
      break;
    // Handle other events...
  }
}
```

### 10.7 Mobile App Architecture

```
React Native App Structure:
├── src/
│   ├── components/
│   │   ├── Question/
│   │   │   ├── QuestionCard.tsx
│   │   │   ├── AnswerOptions.tsx
│   │   │   ├── ExplanationView.tsx
│   │   │   └── ImageViewer.tsx
│   │   ├── Dashboard/
│   │   ├── Analytics/
│   │   └── Common/
│   ├── screens/
│   │   ├── Auth/
│   │   ├── Home/
│   │   ├── Study/
│   │   ├── MockExam/
│   │   ├── Performance/
│   │   └── Settings/
│   ├── services/
│   │   ├── api.ts
│   │   ├── auth.ts
│   │   ├── offline.ts
│   │   └── sync.ts
│   ├── store/
│   │   ├── slices/
│   │   └── index.ts
│   ├── utils/
│   │   ├── spacedRepetition.ts
│   │   └── analytics.ts
│   └── App.tsx

Offline Capabilities:
- SQLite for local question storage
- Queue system for syncing attempts
- Background sync when online
- Conflict resolution strategy
```

### 10.8 Security Considerations

```yaml
Authentication:
  - JWT with short expiry (15 min)
  - Refresh tokens (7 days, rotated)
  - Rate limiting on auth endpoints
  - Account lockout after failed attempts
  - 2FA optional for users

Data Protection:
  - HTTPS everywhere (TLS 1.3)
  - Database encryption at rest
  - PII encryption (user data)
  - GDPR compliance (UK/EU users)
  - Data retention policies

Payment Security:
  - PCI DSS compliance via Stripe
  - No card data stored
  - 3D Secure for authentication
  - Fraud detection (Stripe Radar)

Application Security:
  - OWASP Top 10 mitigations
  - Input validation/sanitization
  - SQL injection prevention (parameterized queries)
  - XSS prevention (content security policy)
  - CSRF tokens
  - Regular security audits
```

---

## 11. Sources and References

### Official Websites
1. [PassMedicine](https://www.passmedicine.com/) - Official platform
2. [Pastest](https://www.pastest.com/) - Official platform
3. [BMJ OnExamination](https://www.onexamination.com/) - Official platform

### Product Pages
4. [PassMedicine MRCP Part 1](https://www.passmedicine.com/mrcp/)
5. [Pastest MRCP Part 1](https://www.pastest.com/products/mrcp-part-1)
6. [BMJ OnExamination MRCP Part 1](https://www.onexamination.com/products/mrcp-part-1)
7. [Pastest MRCP Membership](https://www.pastest.com/products/mrcp-membership)

### Company Information
8. [PassMedicine Company Profile - Tracxn](https://tracxn.com/d/companies/passmedicine/__vVwck35bEPiysQLxiGx433nO4NldK8thLhHLg_bicJ0)
9. [Pastest Company Profile - Tracxn](https://tracxn.com/d/companies/pastest/__NGPglTeMISsS5HLY4EpKvRfAQZU-zouYYzKUw3ckFEs)
10. [Pastest 50th Anniversary](https://www.pastest.com/blogs/news/pastest-celebrates-50th-year)
11. [Pastest Founders Interview](https://www.pastest.com/blogs/news/interview-with-the-pastest-founders)
12. [BMJ OnExamination - Crunchbase](https://www.crunchbase.com/organization/bmj-onexamination)

### Comparison Articles
13. [iatroX - UK Medical Exam Prep Deep Dive](https://www.iatrox.com/blog/medical-exam-prep-amboss-passmedicine-quesmed-pastest-plabable)
14. [iatroX - Free vs Paid Question Banks](https://www.iatrox.com/blog/free-vs-paid-medical-question-banks-uk-mrcp-akt-iatrox-passmedicine-pastest)
15. [Pastest - Best MRCP Part 1 Resources](https://www.pastest.com/blogs/news/the-best-mrcp-part-1-online-revision-resources)
16. [Revising Rubies - Is Passmedicine Good?](https://revisingrubies.com/is-passmedicine-really-any-good/)

### User Reviews
17. [PassMedicine Trustpilot Reviews](https://www.trustpilot.com/review/passmedicine.com)
18. [Pastest Trustpilot Reviews](https://uk.trustpilot.com/review/www.pastest.com)
19. [The Student Room - PassMedicine vs OnExamination](https://www.thestudentroom.co.uk/showthread.php?t=1998914)
20. [The Student Room - PasTest vs PassMedicine vs OnExamination](https://www.thestudentroom.co.uk/showthread.php?t=2313220)

### Mobile Apps
21. [Pastest App - App Store](https://apps.apple.com/gb/app/pastest-written/id1554317254)
22. [Pastest App - Google Play](https://play.google.com/store/apps/details?id=com.pastest.v3.app)
23. [BMJ OnExamination - App Store](https://apps.apple.com/gb/app/bmj-onexam/id544289965)
24. [BMJ OnExamination - Google Play](https://play.google.com/store/apps/details?id=com.bmjgroup.onexamination)
25. [Pastest App Review](https://www.pastest.com/blogs/news/revising-with-the-pastest-app-a-review-by-katie-wood)

### Exam Statistics
26. [MRCP Part 1 January 2024 Performance Report](https://www.thefederation.uk/sites/default/files/2024-02/MRCP(UK) Part 1 24-1 feedback report for the_Liliana Chis.pdf)
27. [MRCP Pass Rates Explained](https://www.thefederation.uk/examinations/guidance-and-information/pass-rates-explained)
28. [GMC PLAB Pass Rates](https://www.gmc-uk.org/registration-and-licensing/join-our-registers/plab/recent-pass-rates-for-plab-1-and-plab-2)

### AI Features
29. [Pastest AI Tutor Launch](https://www.pastest.com/blogs/news/medical-revision-ai-to-the-rescue)
30. [BMJ AI PACES Launch](https://bmjgroup.com/bmj-launches-innovative-ai-powered-exam-revision-tool-for-doctors/)

### Technical Resources
31. [Stripe Healthcare Payments](https://stripe.com/resources/more/healthcare-payment-processing-systems)
32. [Online Examination System Architecture Paper](https://onlinelibrary.wiley.com/doi/10.1155/2021/7849255)

### NHS/Institutional Access
33. [WMUH Library - Medical Examinations](https://www.library.wmuh.nhs.uk/wp/library/medical-examinations/)
34. [Geeky Medics Institutional Licensing](https://geekymedics.com/institutional-licence/)

---

## Appendix A: Glossary of Terms

| Term | Definition |
|------|------------|
| SBA | Single Best Answer - MCQ with one correct option |
| EMQ | Extended Matching Question - Multiple scenarios matching to options |
| BOF | Best of Five - Select best answer from five options |
| MBA | Multiple Best Answer - Select multiple correct answers |
| MRCP | Membership of the Royal Colleges of Physicians |
| MRCGP | Membership of the Royal College of General Practitioners |
| AKT | Applied Knowledge Test (MRCGP component) |
| PLAB | Professional and Linguistic Assessments Board |
| PACES | Practical Assessment of Clinical Examination Skills |
| OSCE | Objective Structured Clinical Examination |
| UKMLA | UK Medical Licensing Assessment |
| IMG | International Medical Graduate |
| RCP | Royal College of Physicians |

---

## Appendix B: Competitor Pricing Quick Reference

### MRCP Part 1
| Platform | 3 months | 6 months | 12 months | Best Value |
|----------|----------|----------|-----------|------------|
| PassMedicine | N/A | ~£45 | N/A | £35/4mo |
| Pastest | £99.99 | £144.99 | £179.99 | £459.99/5yr |
| BMJ OnExamination | £69.99 | £99.99 | £159.99 | 12 months |

### MRCGP AKT
| Platform | 3 months | 6 months | 12 months |
|----------|----------|----------|-----------|
| PassMedicine | N/A | N/A | ~£35/4mo |
| Pastest | ~£99 | ~£145 | ~£180 |
| BMJ OnExamination | ~$70 | ~$110 | N/A |

---

*Report generated by Research Agent*
*Date: December 19, 2025*
*File location: C:\odoo\odoo19\researches\2025-12-19_medical-exam-platforms-competitive-analysis.md*
