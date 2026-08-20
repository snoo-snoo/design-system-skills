# RULE-SPACE-001 — Tokenized Spacing Scale

```text
RULE-SPACE-001
Name: Tokenized Spacing Scale
Category: 01 Foundations / Spacing
Principle: PRINCIPLE-SPACE-001
Recommendation:
  MUST space layout and component internals using a discrete spacing scale
  (design tokens), not arbitrary one-off pixel values.
  SHOULD prefer parent layout/stack gaps over scattering margins on every child.
  SHOULD jump token steps at breakpoints rather than inventing off-scale values.
  MUST NOT invent new spacing numbers when generating UI — pick nearest token.
Reason:
  Ad-hoc margins/paddings break rhythm, hierarchy, and design-system consistency.
Context:
  Product UI layout and component construction (web/admin/enterprise and
  general product surfaces) backed by a spacing scale.
Exceptions:
  Rare optical one-offs (document explicitly).
  Percentage-based page structure splits.
  Third-party embeds outside the system.
Anti-pattern:
  Magic numbers (13px, 27px) mixed through a screen.
  Every child sets its own unique margin instead of a stack/gap.
  Responsive “eyeballed” spacing that ignores the scale.
Evidence:
  - DS-002 Carbon Spacing overview (scale + designing-with-space)
  - DS-005 Primer size/stack tokens
  - DS-003 Card padding token usage (supporting)
  - Wave-A synthesis consensus
Confidence: High
Maturity: CORE
Related Rules: RULE-COLOR-001
PriorityFloor: P4 (system consistency); supports P2 hierarchy
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-SPACE-001 (multi-DS consensus)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-SPACE-001 |
| Source IDs | DS-002, DS-005, DS-003 |
| Normalized from | PRINCIPLE-SPACE-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ ≥2 design systems |
| Accessibility-compatible | ✅ (no conflict) |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ exceptions listed |
| Exact token values invented | ❌ forbidden — use project scale |
