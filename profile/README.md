<div align="center">

# open-templates

**Reusable starter templates with sensible defaults — docs, automation, and pairing where it matters.**

[Browse all repositories](https://github.com/orgs/open-templates/repositories) · [Contributing](https://github.com/open-templates/.github/blob/main/CONTRIBUTING.md) · [Code of Conduct](https://github.com/open-templates/.github/blob/main/CODE_OF_CONDUCT.md)

</div>

---

## How to use

1. Pick a template below (or a **bundle** — frontend + backend).
2. Open the repository and click **Use this template** (or clone and customize).
3. Follow each repo’s `README.md` and `INSTRUCTIONS.md` for setup.

> More templates will be added to each category over time. Watch this org for new bundles and stacks.

---

## Repository templates

Blank GitHub repository shells — community docs, Dependabot, CODEOWNERS, and issue/PR scaffolding. No application code until you add it.

| Template | Summary |
|----------|---------|
| [**github-repo-template**](https://github.com/open-templates/github-repo-template) | Stack-agnostic repo template: markdown docs with cross-links, Dependabot, dependabot-signature workflow, CODEOWNERS, issue & PR templates |

---

## Package templates

Publishable libraries with TypeScript, tests, linting, and CI/CD for npm and GitHub Packages.

| Template | Summary |
|----------|---------|
| [**npm-package-template**](https://github.com/open-templates/npm-package-template) | Production-ready TypeScript npm package — dual ESM/CJS builds (tsup), Vitest, ESLint flat config, automated publish workflows, CodeQL |

---

## Frontend templates

Client apps and UI starters. Pair with a backend template when you need an API.

| Template | Summary |
|----------|---------|
| [**react-supabase-auth-template**](https://github.com/open-templates/react-supabase-auth-template) | React 19 + Vite + Supabase Auth — email/password & Google OAuth, protected routes, health polling, `GET /me` via Worker API |

**Suggested bundle:** [react-supabase-auth-template](https://github.com/open-templates/react-supabase-auth-template) + [cf-hono-supabase-api-template](https://github.com/open-templates/cf-hono-supabase-api-template)

---

## Backend templates

API and worker starters. Pair with a frontend template for full-stack auth flows.

| Template | Summary |
|----------|---------|
| [**cf-hono-supabase-api-template**](https://github.com/open-templates/cf-hono-supabase-api-template) | Cloudflare Worker + Hono + Supabase — public `GET /health`, JWT-protected `GET /me` |

**Suggested bundle:** [cf-hono-supabase-api-template](https://github.com/open-templates/cf-hono-supabase-api-template) + [react-supabase-auth-template](https://github.com/open-templates/react-supabase-auth-template)

---

## Template map

```text
open-templates/
├── Repo Templates
│   └── github-repo-template
├── Package Templates
│   └── npm-package-template
├── Frontend Templates
│   └── react-supabase-auth-template ──┐
└── Backend Templates                  │  full-stack Supabase auth bundle
    └── cf-hono-supabase-api-template ─┘
```

---

<div align="center">

<sub>MIT · Maintained by <a href="https://github.com/open-templates">@open-templates</a></sub>

</div>
