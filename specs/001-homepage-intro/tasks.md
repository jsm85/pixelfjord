---
description: "Task list for homepage intro feature"
---

# Tasks: Homepage Intro

**Input**: Design documents from `/specs/001-homepage-intro/`
**Prerequisites**: plan.md (required), spec.md (required for user stories)

## Phase 1: Setup (Shared Infrastructure)

**Purpose**: Project initialization and basic structure for .NET static site generator with Markdown content

- [x] T001 Create site/ directory structure per plan.md
- [x] T002 Initialize .NET static site generator project (Statiq Web) in site/
- [x] T003 [P] Configure content/ folder for Markdown (site/content/homepage.md)
- [x] T004 [P] Add sample assets (logo, images) to site/input/
- [x] T005 [P] Set up CI/CD pipeline for build and deploy to GitHub Pages
- [x] T006 [P] Configure accessibility and performance checks (e.g., Lighthouse, a11y tools)

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: Core infrastructure that MUST be complete before ANY user story can be implemented

- [ ] T007 Configure Statiq pipelines for Markdown → HTML in site/config/
- [ ] T008 [P] Set up theme support and base layout in site/themes/
- [ ] T009 [P] Add responsive CSS framework or custom CSS in site/themes/
- [ ] T010 [P] Add HTML validation and link checking in tests/

**Checkpoint**: Foundation ready - user story implementation can now begin

---

## Phase 3: User Story 1 - View My Homepage (Priority: P1) 🎯 MVP

**Goal**: Homepage introduces site owner, summarizes skills, interests, and projects, with simple/clean UI, hero banner, and responsive navigation.

**Independent Test**: Visit homepage and confirm intro, skills, interests, and project highlights are present and readable on all devices.

### Implementation for User Story 1

- [ ] T011 [US1] Create homepage.md with intro, skills, interests, and project highlights in site/content/homepage.md
- [ ] T012 [US1] Implement hero banner in site/themes/
- [ ] T013 [US1] Implement navigation (logo top left, nav top right) in site/themes/
- [ ] T014 [US1] Implement scroll-shrinking hero and content reveal in site/themes/
- [ ] T015 [US1] Ensure UI is fully responsive and visually appealing on mobile, tablet, and desktop
- [ ] T016 [US1] Add accessibility features (WCAG AA) to homepage and navigation

**Checkpoint**: Homepage is live, responsive, accessible, and meets all requirements

---

## Phase 4: Polish & Cross-Cutting Concerns

- [ ] T017 [P] Documentation updates in README.md
- [ ] T018 Code cleanup and refactoring
- [ ] T019 Performance optimization (images, CSS, JS)
- [ ] T020 [P] Additional accessibility and device testing

---

## Dependencies & Execution Order

- Setup (Phase 1) → Foundational (Phase 2) → User Story 1 (Phase 3) → Polish (Phase 4)
- All [P] tasks can run in parallel
- User Story 1 is independently testable and MVP

## Implementation Strategy

- Complete Setup + Foundational
- Implement homepage as MVP
- Validate on all devices
- Polish and optimize
