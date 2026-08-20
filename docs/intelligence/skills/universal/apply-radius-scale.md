# SKILL: apply-radius-scale

```text
SKILL: apply-radius-scale

PURPOSE:
Apply border radii from the project’s semantic radius/shape scale only.

SCOPE / WHEN TO USE:
- Styling cards, controls, overlays, images, chips
- Reviewing AI-generated UI for one-off radii

INPUTS:
- Project radius/shape tokens (required if available)
- Component list needing radii

RULES:
1. MUST use semantic radius/shape tokens from the project scale (RULE-RADIUS-SCALE-001).
2. MUST NOT invent arbitrary px radii when tokens exist.
3. SHOULD map like components to the same radius role.
4. SHOULD reserve full/pill for true pills.
5. MAY apply nested-radius craft only as composition guidance on top of the scale.

CONSTRAINTS / DON'T:
- Don't copy Material/Primer numeric values into another product.
- Don't use pill radius on large content panels.

DECISION LOGIC: (P0–P7)
P4 system consistency. Nested optical craft (P5) must not invent off-scale values.

ACCESSIBILITY:
No direct conflict; keep focus rings visible on rounded controls (RULE-FOCUS-001).

OUTPUT REQUIREMENTS:
- Component → radius token map
- Exceptions documented

EDGE CASES:
- Native controls; marketing illustrations; squircles

VALIDATION / SELF-REVIEW:
- [ ] All radii map to tokens (or documented exception)
- [ ] No one-off magic radii
- [ ] Pill usage limited to pill controls

RELATED SKILLS: apply-spacing-scale, apply-semantic-color
SOURCE RULES: RULE-RADIUS-SCALE-001
```
