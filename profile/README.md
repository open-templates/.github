<div align="center">

# open-templates

**Reusable starter templates with sensible defaults — docs, automation, and pairing where it matters.**

[Browse all repositories](https://github.com/orgs/open-templates/repositories) · [Contributing](https://github.com/open-templates/.github/blob/main/CONTRIBUTING.md) · [Code of Conduct](https://github.com/open-templates/.github/blob/main/CODE_OF_CONDUCT.md)

</div>

---

## How to use

1. Pick a **standalone** template below, or a **fullstack pack** (frontend + backend).
2. Open the repository and click **Use this template** (or clone and customize).
3. Follow each repo’s `README.md` and `INSTRUCTIONS.md` for setup.

> More templates will be added over time. Watch this org for new packs and stacks.

---

## Standalone templates

Use on their own — no paired repository required.

### Repository templates

Blank GitHub repository shells — community docs, Dependabot, CODEOWNERS, and issue/PR scaffolding. No application code until you add it.

| Template | Summary |
|----------|---------|
| [**github-repo-template**](https://github.com/open-templates/github-repo-template) | Stack-agnostic repo template: markdown docs with cross-links, Dependabot, dependabot-signature workflow, CODEOWNERS, issue & PR templates |

### Package templates

Publishable libraries with TypeScript, tests, linting, and CI/CD for npm and GitHub Packages.

| Template | Summary |
|----------|---------|
| [**npm-package-template**](https://github.com/open-templates/npm-package-template) | Production-ready TypeScript npm package — dual ESM/CJS builds (tsup), Vitest, ESLint flat config, automated publish workflows, CodeQL |

---

## Fullstack packs

Frontend + backend templates wired to the same auth and API contracts — clone both repos and ship.

### Supabase Auth Pack

| Role | Template | Summary |
|------|----------|---------|
| Frontend | [**react-supabase-auth-template**](https://github.com/open-templates/react-supabase-auth-template) | React 19 + Vite + Supabase Auth — email/password & Google OAuth, protected routes, health polling, `GET /me` |
| Backend | [**cf-hono-supabase-api-template**](https://github.com/open-templates/cf-hono-supabase-api-template) | Cloudflare Worker + Hono + Supabase — public `GET /health`, JWT-protected `GET /me` |

### AI Chat Pack

| Role | Template | Summary |
|------|----------|---------|
| Frontend | [**react-supabase-auth-ai-chat-template**](https://github.com/open-templates/react-supabase-auth-ai-chat-template) | React 19 + Vite + Supabase Auth SPA with **AI chat** — session threads, markdown replies, multi-turn `POST /chat` |
| Backend | [**cf-hono-supabase-gemini-api-template**](https://github.com/open-templates/cf-hono-supabase-gemini-api-template) | Cloudflare Worker + Hono + Supabase + **Gemini** — `GET /health`, JWT `GET /me` & `POST /chat` with conversation history |

---

## Template map

```text
open-templates/
├── Standalone
│   ├── Repo Templates
│   │   └── github-repo-template
│   └── Package Templates
│       └── npm-package-template
└── Fullstack Packs
    ├── Supabase Auth Pack
    │   ├── react-supabase-auth-template (frontend)
    │   └── cf-hono-supabase-api-template (backend)
    └── AI Chat Pack
        ├── react-supabase-auth-ai-chat-template (frontend)
        └── cf-hono-supabase-gemini-api-template (backend)
```

---

<div align="center">

<sub>MIT · Maintained by <a href="https://github.com/open-templates">@open-templates</a></sub>

</div>
