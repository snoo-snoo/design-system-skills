# Candidate → CORE promotion (prod)

**Date:** 2026-08-20  
**Decision:** Product requirement — all remaining CANDIDATE principles (and the last EXPERIMENTAL craft principle) ship as CORE with Universal Skills + adapters.

| Former maturity | Principle | Rule | Skill |
| --- | --- | --- | --- |
| CANDIDATE | RADIUS-001 | RULE-NESTED-RADIUS-001 | nest-corner-radii |
| CANDIDATE | TEXT-ALIGN-001 | RULE-TEXT-ALIGN-001 | align-text-start |
| CANDIDATE | BORDER-RESTRAINT-001 | RULE-BORDER-RESTRAINT-001 | restrain-decorative-borders |
| CANDIDATE | COMPONENT-API-PARITY-001 | RULE-COMPONENT-API-001 | align-design-code-api |
| EXPERIMENTAL | CARD-SURFACE-001 | RULE-CARD-SURFACE-001 | use-card-chrome-sparingly |

## Guardrails retained

- Nested radius remains **composition on top of** RULE-RADIUS-SCALE-001 (CX-001).
- Border/card restraint **cannot** remove P0 focus/contrast/affordance (CX-004 / CX-005).
- Craft rules are P2–P5; Accessibility P0 still wins conflicts.
- Open watches CX-002 / CX-006 unchanged.

## Validation

New checklist: [`../validation/checklists/craft-core.md`](../validation/checklists/craft-core.md)
