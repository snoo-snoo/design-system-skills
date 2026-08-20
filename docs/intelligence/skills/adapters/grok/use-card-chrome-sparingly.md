# ADAPTER: grok/use-card-chrome-sparingly

```text
ADAPTER: grok/use-card-chrome-sparingly
MODEL: grok
UNIVERSAL_SKILL: docs/intelligence/skills/universal/use-card-chrome-sparingly.md
PURPOSE: Use card chrome only when needed; protect contrast
```

## Preamble

Follow the Grok adapter profile (docs/intelligence/skills/adapters/grok/README.md). Be direct. Lead with Verdict and P0 blockers. Use MUST/SHOULD exactly as in the Universal Skill. No filler.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `use-card-chrome-sparingly`
- `{task}` = user task

Do **not** fork Universal Skill RULES.

## Validation checklists

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. `docs/intelligence/validation/checklists/craft-core.md`
4. Extra: design-system, accessibility

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
