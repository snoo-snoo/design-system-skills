# ADAPTER: chatgpt/align-text-start

```text
ADAPTER: chatgpt/align-text-start
MODEL: chatgpt
UNIVERSAL_SKILL: docs/intelligence/skills/universal/align-text-start.md
PURPOSE: Prefer start alignment for multi-line product text
```

## Preamble

Follow the ChatGPT adapter profile (docs/intelligence/skills/adapters/chatgpt/README.md). Use numbered steps and checklists. Include optional JSON validation summary. Map claims to RULE-IDs.

## Invoke

Use [`../invoke-template.md`](../invoke-template.md) with:

- `{MODEL_PREAMBLE}` = this adapter's preamble + profile README
- `{skill}` = `align-text-start`
- `{task}` = user task

Do **not** fork Universal Skill RULES.

## Validation checklists

1. `docs/intelligence/validation/checklists/wave-a-core.md`
2. `docs/intelligence/validation/checklists/wave-b-core.md`
3. `docs/intelligence/validation/checklists/craft-core.md`
4. Extra: ux, consistency

## Output reminder

Finish with skill self-review + Validation Report summary per [`../contract.md`](../contract.md).
