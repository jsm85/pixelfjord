
# Pixelfjord Constitution



## Core Principles

### I. Content as Markdown
All site content MUST be authored in Markdown files. Markdown is the canonical source for all pages, posts, and documentation. No content is maintained solely in HTML or other formats.
*Rationale: Ensures portability, readability, and ease of contribution for all collaborators.*

### II. .NET Static Site Generation
The site MUST be built using a .NET-based static site generator (e.g., Statiq Web). The generator configuration, pipelines, and custom modules MUST be version-controlled and documented.
*Rationale: Leverages .NET ecosystem strengths, enables extensibility, and ensures reproducible builds.*

### III. Automated Build & Deployment
All builds and deployments to GitHub Pages MUST be automated via CI/CD (e.g., GitHub Actions). Manual deployments are prohibited. The build pipeline MUST validate site integrity before publishing.
*Rationale: Guarantees repeatability, reduces human error, and enforces quality gates.*

### IV. Testable & Previewable
Every content or configuration change MUST be previewable in a local or staging environment before merging to main. Automated checks MUST verify site builds without errors and links are valid.
*Rationale: Prevents broken sites, enables safe iteration, and supports contributor confidence.*

### V. Accessibility & Performance
The generated site MUST meet basic accessibility standards (WCAG AA) and performance best practices (e.g., optimized images, minimal JS, semantic HTML). Automated checks SHOULD be used where feasible.
*Rationale: Ensures the site is usable by all and loads quickly for every visitor.*


## Technology & Deployment Constraints

- The only permitted static site generator is a .NET-based tool supporting Markdown (Statiq Web recommended).
- Deployment target is GitHub Pages (via `gh-pages` branch or GitHub Actions Pages workflow).
- All dependencies MUST be open source and compatible with GitHub-hosted runners.
- No server-side code is permitted in production; all output is static HTML/CSS/JS.


## Development Workflow & Quality Gates

- All changes require pull requests and code/content review.
- CI pipeline MUST validate build, run link checks, and (where possible) run accessibility/performance audits.
- No direct commits to main or deployment branches.
- Documentation for build, preview, and contribution MUST be kept up to date in the repository.


## Governance

- This constitution supersedes all other workflow or technical practices for the project.
- Amendments require a pull request, explicit documentation of changes, and a migration/transition plan if breaking.
- All PRs and reviews MUST verify compliance with these principles and constraints.
- Constitution version MUST be incremented according to semantic versioning: MAJOR for breaking/removal, MINOR for new principles/sections, PATCH for clarifications.



<!--
Sync Impact Report
- Version change: 0.0.0 → 1.0.0
- Modified principles: All (template → concrete .NET static site generator best practices)
- Added sections: Technology & Deployment Constraints, Development Workflow & Quality Gates
- Removed sections: None (all template sections concretized)
- Templates requiring updates: plan-template.md (✅), spec-template.md (✅), tasks-template.md (✅)
- Follow-up TODOs: RATIFICATION_DATE (TODO: Set original adoption date)
-->

**Version**: 1.0.0 | **Ratified**: 2026-02-20 | **Last Amended**: 2026-02-20
