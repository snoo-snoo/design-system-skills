# PRINCIPLE-RADIUS-001 — Nested Corner Radius Consistency

```text
Principle:
Nested surfaces should use concentric corner radii related by padding.

Problem:
Identical radii on parent and child with padding > 0 create uneven
concentric corners and a visually “awkward” nested gap.

Recommendation:
When nesting rounded containers, set:
  outer_radius = inner_radius + padding
(equivalently: inner_radius = outer_radius - padding, clamped at ≥ 0).

Why:
Preserves optical concentricity so nested cards/surfaces feel intentional
and consistent across a UI.

Context:
Rounded rectangles/cards/modals with uniform padding on all sides;
product UI surfaces; design-system radius tokens used in nested composition.

Exceptions:
- Corner smoothing / squircles (continuous curvature) — simple px add may not hold optically
- Unequal horizontal vs vertical padding
- Fully pill / stadium shapes (radius ≥ half min-side)
- Brand-expressive intentional mismatch
- Platforms with non-uniform per-corner radii needing independent treatment
- When outer_radius - padding < 0 → use 0 or rethink nesting

Evidence:
- VID-SAMPLE-001 (Zander Whitehurst Reel + LinkedIn transcript)
- Memorisely YouTube short 09T1XTD1FvI
- Secondary restatements: Medium radius-system article; Figma Corner Perfector docs

Confidence:
Medium

Category:
01 Foundations / Radius

StatementClass:
Practice

SpeechVsVisual:
partial

Maturity:
EXPERIMENTAL

PriorityFloor:
P5 (visual hierarchy / craft) — must not override P0 accessibility
```

## Quality Gate (pre-CORE)

| Check | Result |
| --- | --- |
| Clear & reusable | Yes |
| Context + exceptions | Yes (draft) |
| Evidence sufficient for CORE | **No** — educator cluster, not multi-system normative docs yet |
| Objective enough for AI | Yes (formula) |
| Accessibility conflict | None direct |
| Validatable | Yes — compare computed radii vs padding |

**Decision:** Keep EXPERIMENTAL. Next: check whether Carbon/Polaris/Material document nested radius guidance; if ≥1 system + this practice align → CANDIDATE.
