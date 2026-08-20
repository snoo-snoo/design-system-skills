# RULE-TOUCH-001 — Adequate Pointer Targets

```text
RULE-TOUCH-001
Name: Adequate Pointer Targets
Category: 01 Sizing / 06 Accessibility / 03 Components
Principle: PRINCIPLE-TOUCH-TARGET-001
Recommendation:
  MUST size interactive hit areas to meet WCAG 2.2 Target Size (Minimum)
  for applicable controls.
  SHOULD prefer comfortable, thumb-friendly targets for primary mobile actions
  (especially high-stakes flows: payments, auth, irreversible actions).
  MAY enlarge hit area with padding/inset without enlarging the visual glyph.
Reason:
  Small controls cause mis-taps, errors, and exclusion—especially on touch.
Context:
  All pointer UIs; critical for mobile forms and fintech (VID-SAMPLE-004).
Exceptions:
  Inline text links and other WCAG-specified exception paths — still prefer
  larger controls for primary actions.
Anti-pattern:
  Icon-only buttons under minimum target size with no expanded hit area.
  Densely packed adjacent controls that share overlapping inadequate targets.
Evidence:
  - ST-001 WCAG 2.2 SC 2.5.8 Target Size (Minimum)
  - VID-SAMPLE-004 Revolut “Touch Targets” teaching (supporting Practice)
  - DS-005 Primer control size tokens (practical sizing system)
Confidence: High
Maturity: CORE
Related Rules: RULE-FOCUS-001, RULE-FORM-LABEL-001
PriorityFloor: P0
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-TOUCH-TARGET-001 (Wave-A)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-TOUCH-001 |
| Source IDs | ST-001, DS-005, VID-SAMPLE-004 |
| Normalized from | PRINCIPLE-TOUCH-TARGET-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ Standard + DS (+ Practice) |
| Accessibility-compatible | ✅ |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ WCAG exceptions noted |
