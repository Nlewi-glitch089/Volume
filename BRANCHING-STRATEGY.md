Lab 2 – Branching Strategy (TS.5.3)

Overview

This document describes the branching conventions our team follows during development and release.

Branch roles

- main: Production-ready code. Only thoroughly tested, reviewed, and approved changes are merged here. Releases should be tagged on `main`.

- develop: Integration branch for merged feature work. Continuous integration runs here; this branch represents the next release candidate.

- feature/*: Feature branches created from `develop` for new features. Named `feature/<short-description>` (e.g., `feature/login-improvements`). Work is merged back into `develop` via pull requests with code review.

- hotfix/*: Emergency fixes created from `main` to address production issues. After the hotfix is applied and tested, merge into both `main` and `develop` (or create a PR to `develop`) and tag a new release on `main`.

Workflow notes

- Create feature branches from `develop`, keep commits focused and small, and open a PR to `develop` when ready.
- Run CI checks on PRs; require at least one approving review before merging.
- For release preparation, ensure `develop` is stable, then merge into `main` (via PR or release branch) and tag the release.
- For hotfixes, branch from `main`, apply the fix, merge into `main` and `develop`, and create a tag on `main`.

Branch naming examples

- `main` — production
- `develop` — integration
- `feature/user-auth` — new feature
- `hotfix/critical-500` — emergency fix

This strategy keeps `main` clean for production, `develop` for ongoing integration, `feature/*` for isolated feature work, and `hotfix/*` for urgent fixes.
