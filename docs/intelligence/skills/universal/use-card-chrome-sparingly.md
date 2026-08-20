# SKILL: use-card-chrome-sparingly

```text
SKILL: use-card-chrome-sparingly

PURPOSE:
Use filled/bordered cards only when they improve grouping, affordance, or contrast—not by default.

SCOPE / WHEN TO USE:
- Feeds, lists, dashboards, settings layouts
- Auditing “everything is a card” UIs

INPUTS:
- Content blocks, background contrast, interactivity needs

RULES:
1. SHOULD NOT card-wrap every block by default (RULE-CARD-SURFACE-001).
2. SHOULD prefer spacing/typography hierarchy first.
3. MAY add card chrome for containment, affordance, or contrast needs.
4. MUST preserve P0 contrast/readability/target separation (CX-004).

CONSTRAINTS / DON'T:
- Don't remove surfaces that make text or targets fail contrast.
- Don't equate “minimal” with borderless at the cost of a11y.

DECISION LOGIC: (P0–P7)
P0 contrast/readability overrides P5 chrome restraint.

ACCESSIBILITY:
Verify text/control contrast after removing fills/borders.

OUTPUT REQUIREMENTS:
- Blocks with/without card chrome + rationale
- Contrast notes for removals

VALIDATION / SELF-REVIEW:
- [ ] Cards used intentionally
- [ ] Removals checked for contrast/affordance
- [ ] Hierarchy still clear

RELATED SKILLS: restrain-decorative-borders, apply-spacing-scale, apply-semantic-color
SOURCE RULES: RULE-CARD-SURFACE-001, RULE-SPACE-001, RULE-BORDER-RESTRAINT-001
```
