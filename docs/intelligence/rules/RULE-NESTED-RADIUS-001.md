# RULE-NESTED-RADIUS-001 — Nested Corner Radius Consistency

```text
RULE-NESTED-RADIUS-001
Name: Nested Corner Radius Consistency
Category: 01 Foundations / Radius
Principle: PRINCIPLE-RADIUS-001
Recommendation:
  SHOULD keep nested rounded surfaces optically concentric.
  WHEN nesting with uniform padding, prefer:
    outer_radius ≈ inner_radius + padding
    (clamp inner at ≥ 0; snap to RULE-RADIUS-SCALE-001 tokens when a scale exists).
  MUST NOT invent off-scale radii solely to satisfy the formula — pick nearest
  tokens that preserve concentricity.
  MUST NOT override focus/contrast requirements for craft (P0 wins).
Reason:
  Identical parent/child radii with padding > 0 look uneven and unintentional.
Context:
  Nested cards, modals, inset panels with uniform padding.
Exceptions:
  Squircles/continuous curvature; unequal padding; pills/stadiums; intentional
  brand mismatch; per-corner asymmetric radii.
Anti-pattern:
  Same token on parent and padded child with obvious concentric mismatch.
  Computing radii that ignore the project radius scale.
Evidence:
  - VID-SAMPLE-001 (+ educator corpus)
  - CX-001 complementary with Primer/Polaris/Material token scales
  - RULE-RADIUS-SCALE-001
Confidence: Medium–High
Maturity: CORE
Related Rules: RULE-RADIUS-SCALE-001, RULE-SPACE-001
PriorityFloor: P5 craft — never overrides P0
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE by product decision (CANDIDATE → prod); remains
    composition guidance on top of radius scale (CX-001)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Context + exceptions | ✅ |
| Evidence | ✅ Practice + complementary DS scales |
| A11y | ✅ subordinated to P0 |
| Anti-pattern | ✅ |
