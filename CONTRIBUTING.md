# Contributing

## The one rule
**Never commit secrets.** Not even in private repos. Use env vars, GitHub Actions secrets, or Vercel env vars. The `gitleaks` workflow will fail your PR if it finds one.

If you accidentally pushed a secret: rotate it immediately (assume it's compromised), then [purge from history](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository). Don't just delete the file in a follow-up commit — git history retains it.

## Workflow
1. Branch from `main`: `git checkout -b your-name/short-description`
2. Commit small, push often
3. Open a PR; CI must pass; one approval from `@invision-fintech/core` required
4. Squash-merge into `main`

## Naming
- Branches: `<your-name>/<description>`, e.g. `wliu/fix-contact-form`
- Repos: see the table in `README.md`

## Reviews
PRs auto-request review from `@invision-fintech/core` via `CODEOWNERS`. If you need someone specific, @-mention them in the PR.
