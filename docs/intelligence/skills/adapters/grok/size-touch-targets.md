# ADAPTER: grok/size-touch-targets

```text
ADAPTER: grok/size-touch-targets
MODEL: grok
UNIVERSAL_SKILL: docs/intelligence/skills/universal/size-touch-targets.md
PURPOSE: Enforce adequate pointer/touch hit areas
```

## Preamble

Follow the Grok adapter profile (docs/intelligence/skills/adapters/grok/README.md). Be direct. Lead with Verdict and P0 blockers. Use MUST/SHOULD exactly as in the Universal Skill. No filler.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `size-touch-targets`
- `{task}` = user task

Do **not** copy Universal Skill RULES into the prompt as new policy text beyond loading the skill file/path.

## Validation checklists

After output, run:

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. Extra: accessibility (`docs/intelligence/validation/checklists/<name>.md`)

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
