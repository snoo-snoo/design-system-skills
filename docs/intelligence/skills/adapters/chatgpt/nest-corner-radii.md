# ADAPTER: chatgpt/nest-corner-radii

```text
ADAPTER: chatgpt/nest-corner-radii
MODEL: chatgpt
UNIVERSAL_SKILL: docs/intelligence/skills/universal/nest-corner-radii.md
PURPOSE: Keep nested corner radii concentric on the radius scale
```

## Preamble

Follow the ChatGPT adapter profile (docs/intelligence/skills/adapters/chatgpt/README.md). Use numbered steps and checklists. Include optional JSON validation summary. Map claims to RULE-IDs.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `nest-corner-radii`
- `{task}` = user task

Do **not** fork Universal Skill RULES.

## Validation checklists

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. `docs/intelligence/validation/checklists/craft-core.md`
4. Extra: design-system, consistency

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
