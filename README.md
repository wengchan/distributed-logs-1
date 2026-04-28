# template-default

Baseline scaffolding for new repos in the **invision-fintech** organization. When you create a new repo, use this as the template (GitHub web: "Use this template" → New repository).

## What you get

- `CODEOWNERS` routing reviews to `@invision-fintech/core` by default
- `.gitignore` covering Node, Python, env files, and IDE noise
- `.github/workflows/gitleaks.yml` — secret scan on every push and PR (free workaround for GHAS)
- `CONTRIBUTING.md` — naming conventions and the no-secrets rule

## Repo naming convention (read this before naming a new repo)

| Prefix | Visibility | Example | Who has access |
|---|---|---|---|
| `site-*` | Private | `site-main` | All org members (`@invision-fintech/core`) |
| `internal-*` | Private | `internal-billing-tools` | All org members |
| `client-<name>-*` | Private, team-restricted | `client-acme-dashboard` | Specific contractor team only |
| `oss-*` or no prefix | Public | `oss-react-utils` | World-readable; admin-only creation |
| `sandbox-<user>-*` | Private | `sandbox-jdoe-experiment` | Creator + admins |

## Common ops

- New repo from this template: https://github.com/new?template_owner=invision-fintech&template_name=template-default
- Update CODEOWNERS or workflow: edit here, then re-template (existing repos do *not* auto-update)
