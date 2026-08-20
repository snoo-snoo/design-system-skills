# Shared Invoke Template

Copy into a model adapter run. Fill `{…}` placeholders.

```text
{MODEL_PREAMBLE}

You are executing ONE atomic design skill. Do not expand scope.

UNIVERSAL_SKILL_PATH: docs/intelligence/skills/universal/{skill}.md
SOURCE_RULES: (read from that skill — do not invent rules)
PRIORITY_HIERARCHY: P0 Accessibility … P7 Aesthetics
ADAPTER_CONTRACT: docs/intelligence/skills/adapters/contract.md

USER_TASK:
{task}

PROJECT_CONTEXT (optional):
{design system tokens / components / constraints}

INSTRUCTIONS:
1. Load and follow the Universal Skill exactly.
2. Apply P0–P7 when trade-offs appear.
3. Do not invent token values; use project tokens or describe roles.
4. Produce the skill’s OUTPUT REQUIREMENTS.
5. Complete VALIDATION / SELF-REVIEW from the skill.
6. Run Validation Loop checklists listed by the adapter.
7. Return a short Validation Report summary (pass/fail/needs-info).

OUTPUT LANGUAGE: {language or match user}
```
