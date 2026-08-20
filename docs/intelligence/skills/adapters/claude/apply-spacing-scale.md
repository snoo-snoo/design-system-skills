# ADAPTER: claude/apply-spacing-scale

```text
ADAPTER: claude/apply-spacing-scale
MODEL: claude
UNIVERSAL_SKILL: docs/intelligence/skills/universal/apply-spacing-scale.md
PURPOSE: Apply tokenized spacing scale only
```

## Preamble

Follow the Claude adapter profile (docs/intelligence/skills/adapters/claude/README.md). Prefer structured Findings → Changes → Self-review → Validation. Quote RULE-IDs for MUST claims. Never invent tokens.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `apply-spacing-scale`
- `{task}` = user task

Do **not** copy Universal Skill RULES into the prompt as new policy text beyond loading the skill file/path.

## Validation checklists

After output, run:

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. Extra: design-system, consistency (`docs/intelligence/validation/checklists/<name>.md`)

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
