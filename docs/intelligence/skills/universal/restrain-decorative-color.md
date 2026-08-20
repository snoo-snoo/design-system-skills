# SKILL: restrain-decorative-color

```text
SKILL: restrain-decorative-color

PURPOSE:
Limit decorative color; keep strong color for semantic roles and intentional brand moments.

SCOPE / WHEN TO USE:
- Auditing noisy palettes
- Choosing accents vs status/action colors
- Pair with apply-semantic-color

INPUTS:
- UI surfaces/icons under review
- Semantic token roles available

RULES:
1. MUST route meaningful color through semantic tokens (RULE-COLOR-001).
2. MUST NOT use decorative accents where semantic meaning is required (RULE-COLOR-RESTRAINT-001).
3. SHOULD default chrome/text/icons to neutrals.
4. SHOULD add strong color only for meaning or deliberate brand emphasis.
5. MUST preserve contrast (P0).

CONSTRAINTS / DON'T:
- Don't “make it pop” with random accents on errors/destructive actions.
- Don't treat marketing landing palettes as product defaults.

DECISION LOGIC: (P0–P7)
Contrast P0 > semantic roles P4 > decorative preference P7.

ACCESSIBILITY:
Color is never the only error cue; pair with text/icon (RULE-FORM-FEEDBACK-001).

OUTPUT REQUIREMENTS:
- List of color uses classified: semantic / brand / decorative
- Removals or role remaps for decorative misuse

EDGE CASES:
- Charts/categorical viz; high-contrast themes

VALIDATION / SELF-REVIEW:
- [ ] Accents not used for semantic states
- [ ] Neutrals dominate chrome
- [ ] Contrast addressed

RELATED SKILLS: apply-semantic-color, rank-actions
SOURCE RULES: RULE-COLOR-RESTRAINT-001, RULE-COLOR-001
```
