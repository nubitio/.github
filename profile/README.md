# Nubit

Software studio in Peru. We build operational systems for companies that cannot pause the business while the software catches up — invoicing, hosting, admin platforms, and industry SaaS.

**[Sitio](https://nubitio.github.io)** · Arequipa / Peru

## What we ship

| Area | What it is |
| --- | --- |
| **eFact** | Electronic invoicing for Peru (SUNAT) |
| **Nubit Hosting** | Hosting, domains, and provisioning — [nubit-agent](https://github.com/nubitio/nubit-agent) on the server, control plane behind it |
| **Nubit stack** | Symfony + API Platform + React admin. Annotate an entity, get a working CRUD system |

## Open source — Nubit stack

Start here if you want a full admin system in hours:

- **[nubit-skeleton](https://github.com/nubitio/nubit-skeleton)** — template repository. Symfony 7.4 + API Platform 4 + `@nubitio/react-admin`.
- **[nubit-symfony](https://github.com/nubitio/nubit-symfony)** — backend packages (`nubitio/platform`, `nubitio/admin-bundle`, tenant, workflow, sequence).
- **[nubit-react](https://github.com/nubitio/nubit-react)** — `@nubitio/*` frontend packages for API Platform / Hydra.

```bash
gh repo create my-app --template nubitio/nubit-skeleton --private --clone
```

Package splits (`admin-bundle`, `platform`, `tenant-bundle`, …) are **read-only**. Open issues and PRs on `nubit-symfony` or `nubit-react`.

## How we work on GitHub

Default community files, PR and issue templates, and reusable Actions live in this [`.github`](https://github.com/nubitio/.github) repository. They apply to every repo that does not override them.

- Security reports: private advisory on the affected repo (see [SECURITY.md](../SECURITY.md)). Do not file a public issue with exploit details.
- Questions about a public package: GitHub Discussions or an issue on that repo.
- Client / private work stays in private repositories.

## Contact

- Web: [nubitio.github.io](https://nubitio.github.io)
- Security: private advisory on the repository, not email-in-public
