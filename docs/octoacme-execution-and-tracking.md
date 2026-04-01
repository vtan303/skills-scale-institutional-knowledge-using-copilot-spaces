# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies, facilitated by Scrum Master or PM
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone
- Design review syncs (as needed) — ensure design and development alignment
- QA checkpoint (mid-sprint) — assess testing progress and quality readiness

## Role Responsibilities During Execution

### Developers
- Implement features to acceptance criteria
- Participate in code reviews and design discussions
- Flag technical blockers early for removal by Scrum Master
- Coordinate with QA on testability and test scenarios

### QA Lead / Testing Specialist
- Execute test plans and track test results
- Coordinate bug triage and prioritization
- Report quality metrics and readiness status
- Work with Developers to improve test coverage and automation

### Scrum Master
- Facilitate daily standups and team ceremonies
- Identify and help remove impediments
- Track blockers and escalate to PM when needed
- Coach team on process and help optimize workflow

### UX Designer
- Be available for design questions and refinement
- Conduct design reviews during development
- Validate that implementation matches design intent
- Iterate on designs based on user feedback or technical constraints

### Project Manager
- Monitor overall progress against plan and milestones
- Manage stakeholder expectations and communication
- Escalate risks and blockers beyond team control
- Facilitate coordination between teams

### Solutions Architect
- Review technical implementation for alignment with architecture
- Guide decisions on complex technical challenges
- Ensure integration points are properly coordinated

### Product Manager
- Answer feature questions and priority questions
- Validate that delivered features meet acceptance criteria
- Monitor metrics and adjust priorities as needed

## Workflows
- **Use the project board** (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, Design Review (if needed), QA, Done
- **Pull Request workflow:**
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Include design/UX considerations if applicable
  - Run automated tests and linting in CI before requesting review
  - Require at least one code review + one design review (if applicable) before merging
- **Code Review**: Check for correctness, testability, design patterns, and alignment with architecture
- **Design Review**: Ensure implementation matches design intent and user experience standards
- **QA Review**: Validate acceptance criteria and quality standards before marking "Done"

## Quality & Testing
- Unit tests for new logic (Developer responsibility, verified by QA Lead)
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- **QA Sign-off**: QA Lead must validate acceptance criteria before story can be marked "Done"

## Reporting & Metrics
- Track velocity and burndown (coordinated by Scrum Master/PM)
- Monitor success metrics identified in the Project One-pager (Product Manager)
- Use dashboards for key signals (errors, latency, usage)
- Report quality metrics: defect density, test coverage, QA sign-off rate

## Blocker Escalation
- **Level 1**: Team-level triage in daily standup (Scrum Master leads)
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests, lint, and security scanning
- [ ] Regular demos scheduled and demo owners assigned
- [ ] Risk register updated weekly by PM
- [ ] QA Lead has signed off on acceptance criteria for all stories
- [ ] Scrum Master (or PM) is facilitating daily standups consistently
- [ ] Design reviews are scheduled for any UX-impacting work
- [ ] All roles understand their responsibilities and communication channels
