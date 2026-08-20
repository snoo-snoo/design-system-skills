# ADAPTER: grok/restrain-decorative-borders

```text
ADAPTER: grok/restrain-decorative-borders
MODEL: grok
UNIVERSAL_SKILL: docs/intelligence/skills/universal/restrain-decorative-borders.md
PURPOSE: Prefer space over decorative borders; keep P0 edges
```

## Preamble

Follow the Grok adapter profile (docs/intelligence/skills/adapters/grok/README.md). Be direct. Lead with Verdict and P0 blockers. Use MUST/SHOULD exactly as in the Universal Skill. No filler.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `restrain-decorative-borders`
- `{task}` = user task

Do **not** fork Universal Skill RULES.

## Validation checklists

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. `docs/intelligence/validation/checklists/craft-core.md`
4. Extra: design-system, accessibility

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
