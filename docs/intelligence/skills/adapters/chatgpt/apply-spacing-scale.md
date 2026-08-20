# ADAPTER: chatgpt/apply-spacing-scale

```text
ADAPTER: chatgpt/apply-spacing-scale
MODEL: chatgpt
UNIVERSAL_SKILL: docs/intelligence/skills/universal/apply-spacing-scale.md
PURPOSE: Apply tokenized spacing scale only
```

## Preamble

Follow the ChatGPT adapter profile (docs/intelligence/skills/adapters/chatgpt/README.md). Use numbered steps and checklists. Include optional JSON validation summary. Map claims to RULE-IDs.

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
