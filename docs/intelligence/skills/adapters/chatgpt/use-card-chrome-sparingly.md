# ADAPTER: chatgpt/use-card-chrome-sparingly

```text
ADAPTER: chatgpt/use-card-chrome-sparingly
MODEL: chatgpt
UNIVERSAL_SKILL: docs/intelligence/skills/universal/use-card-chrome-sparingly.md
PURPOSE: Use card chrome only when needed; protect contrast
```

## Preamble

Follow the ChatGPT adapter profile (docs/intelligence/skills/adapters/chatgpt/README.md). Use numbered steps and checklists. Include optional JSON validation summary. Map claims to RULE-IDs.

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
