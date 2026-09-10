# nubitio/.github

Organization defaults for [Nubit](https://github.com/nubitio). GitHub copies these into any repository that does not define its own file of the same name.

| Path | Role |
| --- | --- |
| `profile/README.md` | Public org profile at [github.com/nubitio](https://github.com/nubitio) |
| `CONTRIBUTING.md` | Default contributing guide |
| `CODE_OF_CONDUCT.md` | Conduct |
| `SECURITY.md` | How to report vulnerabilities |
| `SUPPORT.md` | Where to ask for help |
| `PULL_REQUEST_TEMPLATE.md` | Default PR body |
| `ISSUE_TEMPLATE/` | Bug / feature forms + contact links |
| `CODEOWNERS` | Default review owner |
| `.github/workflows/reusable-*.yml` | Reusable Actions (`workflow_call`) |
| `workflow-templates/` | Starter workflows in the Actions “new workflow” UI |

## Use a reusable workflow

```yaml
jobs:
  php:
    uses: nubitio/.github/.github/workflows/reusable-ci-php.yml@main
    with:
      php-version: "8.4"
```

A repository that needs different CI should keep its own `.github/workflows` and ignore these templates.

## What this repo cannot do

On GitHub Free, organization rulesets and some org Actions policies are limited. Branch protection still lives on each repository. Secret scanning for new repos is off until the billing plan allows it.

Do not store secrets here.
