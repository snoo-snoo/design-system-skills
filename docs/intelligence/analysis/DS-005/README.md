# Analysis — DS-005 Primer Foundations (Size / Radius)

**Source:** https://primer.style/product/primitives/size/  
**Captured:** 2026-08-20 · **Status:** analyzed (Size primitives slice)

## Claims inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| PR-S1 | Size system is tokenized CSS variables (base sizes 2–128px family) | System Convention | High |
| PR-S2 | Border radius roles: small / medium / large / full (3 / 6 / 12 / 9999px) | System Convention | High |
| PR-S3 | Default/medium radius ≈ 6px; overlays reuse medium radius | System Convention | High |
| PR-S4 | Stack gaps: condensed / normal / spacious (8 / 16 / 24) | System Convention | High |
| PR-S5 | Control sizes and paddings are tokenized by control size tier | System Convention | High |
| PR-S6 | Some control stack gaps adapt for coarse vs fine pointer | System Convention | Medium–High |
| PR-S7 | Focus outline width/offset tokenized | System Convention + A11y | High |

## Radius vs PRINCIPLE-RADIUS-001

Primer publishes a **fixed semantic radius scale**, not a nesting formula. Nested composition using `outer = inner + padding` is **compatible** if the results snap to (or choose among) existing tokens — but Primer does not document that formula.

**Cross-check result:** complementary; no contradiction → keep formula as composition Practice (see principle update).

## Principle candidates

- PRINCIPLE-RADIUS-SCALE-001 (use semantic radius tokens, not ad-hoc px)
- Reinforces PRINCIPLE-SPACE-001 / control sizing
