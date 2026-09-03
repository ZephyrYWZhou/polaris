# Knowledge Branch

Personal notes for learning the Apache Polaris codebase.

## How this differs from existing docs

- `docs/` + `site/` = user-facing guides (how to deploy and use Polaris)
- `spec/` = the API contracts (Iceberg REST Catalog API + Polaris management OpenAPI)
- `AGENTS.md` = coding rules (what reviewers enforce)
- `knowledge/` = **code-level maps and traces** (how the implementation actually works)

## Files

| File | Purpose |
|------|---------|
| _(to be added)_ | Notes accumulate here as learning progresses |

## Module map (starting orientation)

| Module | Role |
|--------|------|
| `polaris-core` | Core domain: entities, catalog model, authorization, persistence abstractions |
| `runtime` | Quarkus service — REST endpoints, wiring, the deployable server |
| `persistence` | Persistence implementations (metastore backends) |
| `api` | Generated API models/interfaces from `spec/` |
| `client` | Client libraries |
| `extensions` | Pluggable extensions |

## Conventions

- Notes are committed with `docs(knowledge): <description>` messages.
- This branch tracks `main` (full code tree) so notes sit alongside the code they describe.
- Keep entries as code-level maps and traces — cite concrete classes/paths so a note can be re-verified against the source.
