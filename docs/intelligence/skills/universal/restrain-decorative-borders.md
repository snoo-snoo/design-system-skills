# SKILL: restrain-decorative-borders

```text
SKILL: restrain-decorative-borders

PURPOSE:
Prefer spacing/typography for hierarchy; use borders only when needed for structure or a11y.

SCOPE / WHEN TO USE:
- Layout chrome reviews
- “Spreadsheet UI” noise reduction
- Pair with apply-spacing-scale and use-card-chrome-sparingly

INPUTS:
- Layout regions, existing borders/dividers
- DS divider components if any

RULES:
1. SHOULD prefer space/proximity over dense decorative borders (RULE-BORDER-RESTRAINT-001).
2. MUST keep borders required for inputs, focus, contrast, and necessary table structure.
3. MAY use DS dividers sparingly when separation is required.
4. MUST NOT strip P0 focus/input edges for aesthetics.

CONSTRAINTS / DON'T:
- Don't remove affordance borders to chase a flat look.

DECISION LOGIC: (P0–P7)
P0 focus/contrast > P2 hierarchy > P5 craft.

ACCESSIBILITY:
Borders for focus/inputs/tables often required.

OUTPUT REQUIREMENTS:
- Borders kept vs removed with rationale
- Spacing substitutions noted

VALIDATION / SELF-REVIEW:
- [ ] Decorative border density reduced where safe
- [ ] P0 borders intact
- [ ] Hierarchy still clear via space/type

RELATED SKILLS: apply-spacing-scale, use-card-chrome-sparingly, ensure-visible-focus
SOURCE RULES: RULE-BORDER-RESTRAINT-001, RULE-SPACE-001, RULE-FOCUS-001
```
