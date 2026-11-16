# developer-skills

Catalog of reusable developer skills (Claude Agent Skills). The catalog is heterogeneous, so skills are grouped by **domain category**.

## Layout

```
developer-skills/
├── README.md
└── skills/
    └── <category>/
        └── <skill-name>/
            ├── SKILL.md            # required: frontmatter (name, description) + instructions
            ├── references/         # optional: deep-dive docs and code patterns, loaded on demand
            ├── scripts/            # optional: runnable helpers
            └── assets/             # optional: templates, fixtures
```

Rules
- One skill per folder; folder name = `name` in the frontmatter (kebab-case).
- `description` states **what it does and when to trigger it**; this is what decides whether the skill is used.
- Keep `SKILL.md` focused; move long code and rarely-needed detail to `references/`.
- Pick the category by the skill's **primary topic**; create a new category only when no existing one fits.

## Categories

| Category | Scope |
|---|---|
| `mcp/` | Designing, building, securing and testing MCP servers and tools |
| `agents/` | Agent design, prompting, evaluation, orchestration *(planned)* |
| `devops/` | CI/CD, deployment, containers, GitOps *(planned)* |
| `backend/` | Service design, APIs, databases, search pipelines *(planned)* |
| `security/` | Secure design, secrets, threat modelling *(planned)* |
| `docs-process/` | Documentation, issue/epic conventions, review checklists *(planned)* |

## Skills

| Skill | Category | Summary |
|---|---|---|
| [`mcp-tools-development`](skills/mcp/mcp-tools-development/SKILL.md) | mcp | Design philosophy, read/write tool safety, response envelope, server-side auth/IDs/concurrency/timeouts, binary-by-reference, annotations, untrusted data, checklist |

## Adding a skill

1. Create `skills/<category>/<skill-name>/SKILL.md` with frontmatter.
2. Add references/scripts as needed.
3. Add a row to the **Skills** table above.
