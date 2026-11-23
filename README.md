# developer-skills

Catalog of reusable developer skills (Agent Skills).

## Layout

```
developer-skills/
├── README.md
└── skills/
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

## Adding a skill

1. Create `skills/<skill-name>/SKILL.md` with frontmatter.
2. Add references/scripts as needed.
3. Add a row to the **Skills** table above.
