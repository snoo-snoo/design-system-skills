# Schema: Model Adapter

Adapters wrap Universal Skills for a specific model. They **must not** fork or rewrite Canonical Rules / Universal Skill RULES.

```text
ADAPTER: <model-id>/<skill-id or _profile>

MODEL:
  id: claude | grok | chatgpt
  family: Anthropic Claude / xAI Grok / OpenAI ChatGPT
  notes:

UNIVERSAL_SKILL: docs/intelligence/skills/universal/<skill>.md
SOURCE_RULES: (inherit from Universal Skill — do not restate as new law)

PROMPTING STYLE:
  - system / developer framing preferences
  - tool-use expectations (if any)
  - verbosity / structure defaults

INVOCATION TEMPLATE:
  (how to load the Universal Skill + user task)

OUTPUT SHAPING:
  - preferred sections / JSON vs prose
  - must still satisfy Universal Skill OUTPUT REQUIREMENTS

VALIDATION HOOK:
  - run docs/intelligence/validation/ loop after output
  - attach checklist IDs

CONSTRAINTS:
  - No rule invention
  - No token-value invention
  - P0–P7 hierarchy unchanged
  - On conflict, Universal Skill + CORE Rule win over adapter tone
```

## Profile vs skill adapter

| Type | File | Purpose |
| --- | --- | --- |
| Model profile | `adapters/<model>/README.md` | Shared voice, safety, citation habits |
| Skill adapter | `adapters/<model>/<skill>.md` | Thin invoke wrapper for one Universal Skill |
