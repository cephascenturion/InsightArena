# InsightArena Wave Program Plan

## Overview
The Wave Program runs scoped sprint cycles where maintainers post issues and contributors pick them up. This plan defines the work types, scoping rules, contribution flow, review standards, and release cadence for InsightArena. It is designed to keep contributions focused, reviewable, and aligned with project goals.

## Program Goals
- Deliver reliable features and fixes in predictable sprint cycles.
- Grow contributor base through well-scoped, approachable issues.
- Maintain high code quality, test coverage, and documentation.
- Reduce friction in onboarding and review.

## Work Types

### Bug Fixes
- Reproduce and fix defects in backend services, smart contracts, or frontend.
- Include regression tests and clear reproduction steps.
- Scope: single root cause, minimal diff.
- Required: failing test before fix when feasible, root-cause note in PR.

### New Features
- Add endpoints, contract methods, or UI components aligned with roadmap.
- Must include tests, docs, and migration notes when applicable.
- Scope: one cohesive capability per issue.
- Break large features into milestones with independent deliverables.

### Documentation
- Improve README, API docs, setup guides, and inline comments.
- Fix inaccuracies, add examples, and clarify workflows.
- Include screenshots or curl examples where helpful.

### Testing
- Increase coverage for services, contracts, and components.
- Add unit, integration, and E2E tests.
- Focus on edge cases, error paths, and concurrency.
- Prefer deterministic tests; avoid flaky timing dependencies.

### Refactoring
- Improve code quality without changing behavior.
- Requires tests to guard regressions.
- Explain motivation and safety checks in PR.

### Performance
- Optimize queries, caching, and rendering.
- Include benchmarks and before/after metrics.
- Avoid premature optimization; target measured bottlenecks.

### Security
- Address vulnerabilities, input validation, and auth checks.
- Follow responsible disclosure practices.
- Never commit secrets; rotate exposed credentials immediately.

### DevOps and Tooling
- Improve CI pipelines, build scripts, and developer experience.
- Keep changes backward compatible and documented.

## Scoping Rules
- Issues must be self-contained and completable within one sprint.
- Each issue lists acceptance criteria, files in scope, and estimated effort.
- Avoid cross-cutting changes unless explicitly marked.
- Prefer small PRs; large changes split into stacked PRs.

## Contribution Flow
1. Pick an issue labeled `wave`.
2. Comment to claim; maintainers assign.
3. Fork, branch from `main`, implement with tests.
4. Open PR referencing issue; keep changes focused.
5. Address review feedback; maintainers merge.
6. Update docs and changelog entries when needed.

## Branching and Commits
- Branch names: `feat/`, `fix/`, `docs/`, `test/`, `refactor/`.
- Commit messages follow conventional commits.
- Squash merge preferred for clean history.

## Review Standards
- At least one maintainer approval.
- CI green: lint, typecheck, tests.
- No unresolved comments.
- Scope matches issue; no unrelated edits.

## Definition of Done
- Tests pass locally and in CI.
- Documentation updated.
- No unrelated changes.
- PR approved by maintainer.
- Issue closed with summary comment.

## Sprint Cadence
- Sprints run two weeks.
- Planning at start; demo and retro at end.
- Issues triaged weekly; blockers escalated promptly.

## Labels
- `bug`, `feature`, `docs`, `tests`, `refactor`, `perf`, `security`, `devops`, `wave`, `good-first-issue`.

## Communication
- Use issue comments for technical discussion.
- Use PR descriptions for implementation rationale.
- Respect maintainers' review timelines.

## Quality Gates
- Minimum test coverage thresholds enforced in CI.
- Lint and typecheck must pass.
- Security scans run on PRs.

## Onboarding
- New contributors start with `good-first-issue`.
- Maintainers provide starter context and pointers.
- Pairing available on request.

## Metrics
- Track cycle time, PR size, and test coverage.
- Review throughput and contributor retention.
- Adjust scoping based on data.

## Risk Management
- Identify dependencies early.
- Flag breaking changes clearly.
- Provide rollback plans for risky changes.

## Release Process
- Tag releases after sprint completion.
- Publish changelog and migration notes.
- Deploy to staging then production.

## Conclusion
The Wave Program succeeds when issues are scoped, contributions are focused, and reviews are timely. Follow this plan to keep InsightArena moving forward efficiently.
