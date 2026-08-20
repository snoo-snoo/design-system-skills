# ADAPTER: grok/align-design-code-api

```text
ADAPTER: grok/align-design-code-api
MODEL: grok
UNIVERSAL_SKILL: docs/intelligence/skills/universal/align-design-code-api.md
PURPOSE: Map design props to implementation component API
```

## Preamble

Follow the Grok adapter profile (docs/intelligence/skills/adapters/grok/README.md). Be direct. Lead with Verdict and P0 blockers. Use MUST/SHOULD exactly as in the Universal Skill. No filler.

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
