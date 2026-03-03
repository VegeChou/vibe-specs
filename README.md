# vibe-specs

Unified API rule assets for LLM-assisted development.

## Project Structure

```text
.
├── .githooks/
├── .github/workflows/
├── docs/
│   ├── api-spec.md
│   └── new-project-setup.md
├── rules/
│   ├── unified-api.openapi.yaml
│   └── unified-api.human.md
└── scripts/
    ├── bootstrap-api-rules.sh
    ├── install-githooks.sh
    └── sync-api-docs.sh
```

## Entry Points

- Machine-readable contract: `rules/unified-api.openapi.yaml`
- Human-readable generated doc: `rules/unified-api.human.md`
- Spec overview: `docs/api-spec.md`
- New project onboarding: `docs/new-project-setup.md`

## Common Commands

```bash
# Regenerate human-readable rules from OpenAPI
bash scripts/sync-api-docs.sh

# Install local git hooks
bash scripts/install-githooks.sh

# Bootstrap these rule assets into another repository
bash scripts/bootstrap-api-rules.sh /path/to/target-project
```

