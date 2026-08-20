# ADAPTER: grok/restrain-decorative-color

```text
ADAPTER: grok/restrain-decorative-color
MODEL: grok
UNIVERSAL_SKILL: docs/intelligence/skills/universal/restrain-decorative-color.md
PURPOSE: Limit decorative color; keep semantic color meaningful
```

## Preamble

Follow the Grok adapter profile (docs/intelligence/skills/adapters/grok/README.md). Be direct. Lead with Verdict and P0 blockers. Use MUST/SHOULD exactly as in the Universal Skill. No filler.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `restrain-decorative-color`
- `{task}` = user task

Do **not** copy Universal Skill RULES into the prompt as new policy text beyond loading the skill file/path.

## Validation checklists

After output, run:

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. Extra: design-system, accessibility

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
