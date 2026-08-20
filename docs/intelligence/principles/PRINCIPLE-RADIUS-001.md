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
CORE (formalized as RULE-NESTED-RADIUS-001, 2026-08-20 — prod promotion)

| Source | Nested formula? | Radius approach |
| --- | --- | --- |
| VID-SAMPLE-001 | Yes — teaches formula | Educator practice |
| DS-005 Primer | No | Fixed semantic tokens (sm/md/lg/full) |
| DS-003 Polaris | No | Shape tokens required; Card defaults fixed |
| DS-002 Carbon | Not found on captured pages | Spacing/color documented; radius page missing |

**Resolution (CX-001):** Complementary, not contradictory. Systems standardize **tokenized radius scales**; the nesting formula is a **composition rule** for choosing nested token values (or computed radii that then snap to tokens). Does not alone define the scale.

## Quality Gate (pre-CORE)

| Check | Result |
| --- | --- |
| Clear & reusable | Yes |
| Context + exceptions | Yes |
| Evidence for CORE | **Not yet** — strong Practice/CANDIDATE; needs broader independent system doc or synthesis pass |
| Objective for AI | Yes |
| Accessibility conflict | None direct |
| Validatable | Yes |

**Decision:** Promoted to **CORE** (RULE-NESTED-RADIUS-001) as composition guidance on top of radius scale.
