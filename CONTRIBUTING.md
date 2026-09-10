# Contributing to Nubit repositories

This file is the org default. A repository may replace it with a more specific guide.

## Before you start

1. Check existing issues and discussions on the **canonical** repository:
   - Backend PHP packages → [nubit-symfony](https://github.com/nubitio/nubit-symfony)
   - Frontend `@nubitio/*` → [nubit-react](https://github.com/nubitio/nubit-react)
   - Starter template → [nubit-skeleton](https://github.com/nubitio/nubit-skeleton)
   - Hosting agent → [nubit-agent](https://github.com/nubitio/nubit-agent)
2. Read-only split repos (`admin-bundle`, `platform`, `tenant-bundle`, `api-platform`, `workflow-bundle`, `sequence-bundle`) do not accept PRs. Open them on `nubit-symfony`.
3. Security issues: follow [SECURITY.md](SECURITY.md). Never open a public issue with a working exploit.

## Pull requests

- One concern per PR. Do not mix a refactor with a feature.
- Target `main` unless the repo documents another branch.
- Fill in the PR template. Link the issue if there is one.
- Tests and lint must pass on the default CI workflow.
- Do not commit secrets, `.env` with real credentials, or customer data.
- Keep the diff reviewable. If generated files change, say so in the description.

### Commit messages

Prefer a short imperative subject (`Fix grid filter on empty Hydra collections`) over `wip` or `fix stuff`. Conventional Commits (`feat:`, `fix:`, `docs:`) are welcome where the repo already uses them (especially `nubit-react` / `nubit-symfony` releases).

## Issues

Use the issue forms when they appear. Include:

- Expected vs actual behaviour
- Version (package line, commit, or template date)
- Minimal reproduction, not a production dump

## Code of conduct

[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
