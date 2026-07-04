# Instructions — open-templates `.github`

Guide for maintainers and coding agents working on the **organization meta-repository** (`open-templates/.github`), not on individual template repos.

## What this repository is

| Path | Role |
|------|------|
| [`profile/README.md`](profile/README.md) | **Public org profile** — template catalog shown on [github.com/open-templates](https://github.com/open-templates) |
| [`README.md`](README.md) | Landing page when browsing this repo |
| [`INSTRUCTIONS.md`](INSTRUCTIONS.md) | This file — how to maintain the catalog |
| [`CHANGELOG.md`](CHANGELOG.md) | Notable changes to the org meta-repo |
| [`docs/`](docs/README.md) | Reference for workflows and GitHub UI files **in this repo** |
| Community files | `CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md` — org-wide defaults |

Template source code and per-template docs live in **separate repositories** (e.g. `github-repo-template`, `react-supabase-auth-template`).

---

## Template categories

Keep the catalog grouped into these sections (expand each over time):

| Category | Purpose | Current template(s) |
|----------|---------|------------------------|
| **Repository templates** | Empty repo shells — docs, Dependabot, CODEOWNERS | `github-repo-template` |
| **Package templates** | Publishable libraries — build, test, publish CI | `npm-package-template` |
| **Frontend templates** | Client apps and UI starters | `react-supabase-auth-template` |
| **Backend templates** | APIs, workers, services | `cf-hono-supabase-api-template` |

When a frontend and backend template are designed to work together, call that out as a **suggested bundle** in `profile/README.md` (as with the Supabase auth pair).

---

## Adding a new template to the org index

1. **Create or publish** the template repository under the `open-templates` org.
2. **Choose the category** (or add a new category section only if it does not fit the four above — discuss first).
3. **Update [`profile/README.md`](profile/README.md)**:
   - Add a row to the category table: **name** (link), **one-line summary**.
   - Update the ASCII **Template map** if useful.
   - Mention bundles if the new repo pairs with an existing one.
4. **Update [`README.md`](README.md)** quick-reference tables to match.
5. **Record the change** in [`CHANGELOG.md`](CHANGELOG.md) under `### Added` or `### Changed`.
6. **Org profile description** (optional): GitHub org **Settings → Profile** — keep in sync with the tagline in `profile/README.md`.

Do **not** duplicate full template READMEs in the org profile; link out and summarize in one sentence.

---

## Editing the org profile README

[`profile/README.md`](profile/README.md) supports GitHub-flavored markdown plus limited HTML (e.g. `<div align="center">`).

Guidelines:

- Lead with what **open-templates** is and how to use templates.
- One table per category; consistent columns: **Template** | **Summary**.
- Note that categories will grow (“more coming”).
- Keep links absolute to `https://github.com/open-templates/<repo>`.
- Avoid stack-specific walls of text — detail belongs in each template repo.

Preview: push to `main` and open [github.com/open-templates](https://github.com/open-templates) (may take a short moment to refresh).

---

## CHANGELOG (this repo)

[CHANGELOG.md](CHANGELOG.md) tracks **org meta-repo** changes (profile index, org docs, shared `.github` config)—not releases of individual templates. Each template repo maintains its own changelog.

Use **feature-based batches** and [conventional commits](https://www.conventionalcommits.org/):

| Prefix | Typical use |
|--------|-------------|
| `docs:` | Profile index, README, INSTRUCTIONS |
| `feat:` | New org-wide workflow or template listing |
| `chore:` | Dependabot, housekeeping |

Example entry when adding a template:

```markdown
## [0.2.0] - 2026-07-04

### Added
- Frontend template: `next-starter-template` in org profile index
```

---

## Automation in this repo

Same pattern as [github-repo-template](https://github.com/open-templates/github-repo-template):

| Asset | Role |
|-------|------|
| `.github/dependabot.yml` | Dependency update PRs |
| `.github/workflows/dependabot-signature.yml` | `Co-authored-by` on Dependabot commits |
| `.github/CODEOWNERS` | Review ownership |

Details: [docs/README.md](docs/README.md).

---

## Agent checklist

When asked to update the org catalog:

1. Read [`profile/README.md`](profile/README.md) and this file.
2. Confirm the template repo exists and which **category** it belongs to.
3. Add a table row + optional bundle note; sync [`README.md`](README.md).
4. Append [`CHANGELOG.md`](CHANGELOG.md).
5. Do not modify individual template repos unless explicitly scoped to that task.

---

## Repository documents

[README](README.md) | **INSTRUCTIONS** | [CHANGELOG](CHANGELOG.md) | [CONTRIBUTING](CONTRIBUTING.md) | [SECURITY](SECURITY.md) | [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)
