# SKILL: align-text-start

```text
SKILL: align-text-start

PURPOSE:
Prefer start alignment for multi-line product UI text; reserve centering for short titles.

SCOPE / WHEN TO USE:
- Body copy, forms, lists, descriptions
- Auditing centered text blocks

INPUTS:
- Text blocks + intended alignment
- Locale/direction (LTR/RTL)

RULES:
1. SHOULD start-align multi-line readable content (RULE-TEXT-ALIGN-001).
2. MUST NOT default long centered paragraphs in product UI.
3. MAY center short headlines / single-line labels / hero empty-state titles.
4. MUST use logical start/end in RTL.

CONSTRAINTS / DON'T:
- Don't center form labels/help as multi-line stacks.

DECISION LOGIC: (P0–P7)
P2 hierarchy/scanability over P7 aesthetic centering.

ACCESSIBILITY:
Improves scanning; does not replace contrast/focus rules.

OUTPUT REQUIREMENTS:
- Block → alignment map
- Centered exceptions justified

VALIDATION / SELF-REVIEW:
- [ ] Multi-line body/forms are start-aligned
- [ ] Centered usage is short/intentional
- [ ] RTL logical alignment considered

RELATED SKILLS: label-form-fields, apply-spacing-scale
SOURCE RULES: RULE-TEXT-ALIGN-001
```
