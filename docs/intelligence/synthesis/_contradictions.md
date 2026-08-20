# Contradiction Log

Conflicts discovered during cross-source synthesis. Do not invent consensus.

| ID | Status | Topic |
| --- | --- | --- |
| CX-001 | resolved-complementary | Nested radius formula (VID-SAMPLE-001) vs DS fixed radius token scales (Primer/Polaris). Complementary: tokens define the scale; formula guides nested composition. Formula stays CANDIDATE, not CORE. |
| CX-003 | resolved-default | Floating labels (VID-SAMPLE-004) vs persistent-label a11y consensus. **Default:** RULE-FORM-LABEL-001 (persistent). Floating labels = non-default brand exception only. |

## Open watches

| ID | Status | Topic |
| --- | --- | --- |
| CX-002 | open | Carbon disabled contrast policy (“not subject to WCAG contrast”) vs strict reading of non-text contrast — capture Carbon a11y page before elevating related claims |
| CX-004 | open | Borderless cards (VID-SAMPLE-003) vs readability/contrast needs — CARD-SURFACE-001 kept EXPERIMENTAL with P0 override |
| CX-005 | noted | “When do you draw a line?” (VID-SAMPLE-006) — covered by BORDER-RESTRAINT exceptions (inputs, tables, focus, density) |
| CX-006 | open-documented | Atlassian guidance to avoid disabled buttons (esp. form submit) vs common disabled-primary patterns. **Working stance:** prefer validation/explanation over silent disable; not a CORE ban on all disabled controls. |

## Rule

If two HIGH-confidence sources conflict:

1. Prefer P0 Accessibility / Usability
2. Split by Context (platform, density, product type)
3. Keep both as scoped rules rather than forcing one global rule
