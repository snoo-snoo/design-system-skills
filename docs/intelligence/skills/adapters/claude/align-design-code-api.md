# ADAPTER: claude/align-design-code-api

```text
ADAPTER: claude/align-design-code-api
MODEL: claude
UNIVERSAL_SKILL: docs/intelligence/skills/universal/align-design-code-api.md
PURPOSE: Map design props to implementation component API
```

## Preamble

Follow the Claude adapter profile (docs/intelligence/skills/adapters/claude/README.md). Prefer structured Findings → Changes → Self-review → Validation. Quote RULE-IDs for MUST claims. Never invent tokens.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `align-design-code-api`
- `{task}` = user task

Do **not** fork Universal Skill RULES.

## Validation checklists

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. `docs/intelligence/validation/checklists/craft-core.md`
4. Extra: design-system, consistency

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
