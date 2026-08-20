# Analysis — DS-003 Polaris Foundations (Shape / Card defaults)

**Sources (partial; some Polaris URLs timed out / 404 during capture):**  
- Stylelint docs requiring `--p-border-radius-*` tokens  
- Card component docs (default radius/padding/shadow)  
**Captured:** 2026-08-20 · **Status:** analyzed (thin but usable)

## Claims inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| PO-R1 | Use Polaris shape tokens (`--p-border-radius-*`) instead of hard-coded px/rem radii | System Convention | High |
| PO-R2 | Hard-coded border radii are lint-discouraged for Admin consistency | System Convention | High |
| PO-C1 | Default Card: ~8px radius, `space-400` (16px) padding, surface bg + shadow | System Convention | High |
| PO-C2 | Card padding/radius can vary by breakpoint (`roundedAbove`, responsive padding) | System Convention | Medium |

## Radius vs PRINCIPLE-RADIUS-001

Default Card example: radius 8 + padding 16. Nested card-inside-card with same tokens would **not** satisfy `outer = inner + padding` unless designers pick different radius tokens per nest level (e.g. outer 24 / inner 8 with pad 16). Polaris enforces **token usage**, not concentric math.

**Cross-check:** formula is optional composition guidance on top of token scales → CX-001 marked complementary.

## Caveats

- Full tokens/border page 404’d via mirror; re-fetch stable token table in a follow-up capture.
- Do not copy Shopify visual values as universal defaults.
