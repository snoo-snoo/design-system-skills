# SKILL: nest-corner-radii

```text
SKILL: nest-corner-radii

PURPOSE:
Keep nested rounded surfaces optically concentric using padding-aware radii
that still snap to the project radius scale.

SCOPE / WHEN TO USE:
- Nested cards, inset panels, modals with inner surfaces
- Reviewing awkward nested corner gaps

INPUTS:
- Parent/child surfaces, padding, available radius tokens

RULES:
1. SHOULD keep nested corners concentric (RULE-NESTED-RADIUS-001).
2. WHEN padding is uniform, prefer outer ≈ inner + padding (clamp ≥ 0).
3. MUST snap to RULE-RADIUS-SCALE-001 tokens when a scale exists.
4. MUST NOT invent off-scale values just to hit the formula.
5. MUST NOT weaken focus/contrast for craft.

CONSTRAINTS / DON'T:
- Don't apply the formula blindly to pills, squircles, or unequal padding.

DECISION LOGIC: (P0–P7)
P4 scale tokens beat formula purity; P5 craft; P0 a11y always wins.

ACCESSIBILITY:
No direct conflict; preserve visible focus on rounded controls.

OUTPUT REQUIREMENTS:
- Parent/child radius token choices + padding math notes
- Exceptions listed

VALIDATION / SELF-REVIEW:
- [ ] Concentric intent addressed
- [ ] Values on scale (or documented exception)
- [ ] No P0 regressions

RELATED SKILLS: apply-radius-scale, apply-spacing-scale
SOURCE RULES: RULE-NESTED-RADIUS-001, RULE-RADIUS-SCALE-001
```
