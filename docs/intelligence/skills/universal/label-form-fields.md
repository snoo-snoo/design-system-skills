# SKILL: label-form-fields

```text
SKILL: label-form-fields

PURPOSE:
Ensure every form field has a persistent, visible label and does not rely on
placeholder-only or disappearing label patterns.

SCOPE / WHEN TO USE:
- Creating or auditing forms (settings, onboarding, checkout, fintech)
- Reviewing floating-label or placeholder-as-label designs
- Resolving CX-003-style conflicts (brand floating labels vs a11y default)

INPUTS:
- Field list (name, type, required, hint)
- Current label strategy (persistent / floating / placeholder)
- Locale / truncation constraints

RULES:
1. MUST attach a persistent visible label to each data-entry field (RULE-FORM-LABEL-001).
2. MUST NOT use placeholder as the only label.
3. SHOULD put short labels above/beside controls in reading order.
4. SHOULD use placeholder only for format examples.
5. SHOULD default to persistent labels; treat floating labels as non-default exceptions.

CONSTRAINTS / DON'T:
- Don't remove labels to “save space” on high-stakes forms.
- Don't let floating labels become unreadable while typing.
- Don't ship icon-only fields without visible text + accessible name.

DECISION LOGIC: (P0–P7)
P0 labeling wins over P6–P7 brand floating-label trends (CX-003).

ACCESSIBILITY:
Aligns with WCAG 3.3.2 Labels or Instructions. Labels must remain available
to AT even when visually specialized.

OUTPUT REQUIREMENTS:
- Field → label mapping
- Hint vs label separation
- Explicit list of any approved exceptions

EDGE CASES:
- Search fields with visible legend
- OTP / PIN grouped inputs sharing one label
- RTL layout (logical start/end placement)

VALIDATION / SELF-REVIEW:
- [ ] Every field has a persistent visible label
- [ ] No placeholder-only labels on data-entry fields
- [ ] Hints are not substituted for labels
- [ ] Exceptions documented

RELATED SKILLS: size-touch-targets, ensure-visible-focus
SOURCE RULES: RULE-FORM-LABEL-001
```
