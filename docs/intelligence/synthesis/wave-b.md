# Wave B — Cross-Source Synthesis

**Date:** 2026-08-20  
**Scope:** B1 Actions · B2 Forms & validation feedback · Foundations hardening (Material + Atlassian) · CANDIDATE promotions  
**Inputs:** DS-001 · DS-004 · DS-003-forms · prior Wave A principles/rules · [_contradictions.md](_contradictions.md)

---

## 1. Foundations hardening (already CORE)

| Rule | New evidence | Effect |
| --- | --- | --- |
| RULE-SPACE-001 | Atlassian space tokens + proximity/hierarchy; Material spacing scale | Confidence ↑; changelog cite |
| RULE-COLOR-001 | Atlassian color roles/themes/contrast; Material tokenized color | Confidence ↑; changelog cite |

No rule text rewrite required beyond changelog + evidence append.

---

## 2. Consensus → new / promoted CORE

| Theme | Consensus | Evidence mix | Rule |
| --- | --- | --- | --- |
| Radius scale | Use a limited semantic radius/shape scale, not one-off px | Primer + Polaris + Material shape scale | **RULE-RADIUS-SCALE-001** |
| Color restraint | Prefer semantic/meaningful color; avoid decorative accent misuse | Carbon “sparingly” + Atlassian accent-vs-semantic + VID-002 | **RULE-COLOR-RESTRAINT-001** |
| Form feedback | Timely visible focus/validation/progress feedback; field errors in context | ST-003 #1 + Polaris inline error/AT association + FORM-LABEL/FOCUS | **RULE-FORM-FEEDBACK-001** |
| Action hierarchy | One primary CTA per area; danger only for destructive confirms | Atlassian button appearances (+ common DS pattern) | **RULE-ACTION-001** |

---

## 3. Remain CANDIDATE / EXPERIMENTAL

| Principle | Why still held |
| --- | --- |
| RADIUS-001 (nested formula) | Complementary craft (CX-001); not a system law |
| TEXT-ALIGN-001 | Craft; limited formal DS pages in this wave |
| BORDER-RESTRAINT-001 | Craft; exceptions already protect P0 |
| COMPONENT-API-PARITY-001 | Governance practice; needs more DS eng docs |
| CARD-SURFACE-001 | EXPERIMENTAL (CX-004) |
| “Never disable buttons” (ATL-B5) | Strong a11y caution; not yet multi-source CORE |

---

## 4. Context splits

| Topic | Default | Context exception |
| --- | --- | --- |
| Validation timing | Prefer after field interaction (blur) + on submit | Live validation for tight formats (OTP) if not noisy |
| Primary buttons | One per view/region | Multi-column dashboards may have one primary **per independent region** |
| Danger buttons | Final destructive confirm | Non-destructive “remove from list” may use default + confirm modal |
| Accent color | Decorative only | Charts / categorical data viz |

---

## 5. Contradiction updates

| ID | Wave B note |
| --- | --- |
| CX-001 | Unchanged complementary |
| CX-002 | Still open — Atlassian contrast cites don’t resolve Carbon disabled policy |
| CX-003 | Already resolved |
| CX-004 | Still open |
| CX-006 | **New watch** — “Avoid disabled buttons” (Atlassian) vs widespread disabled-submit patterns → document as guidance CANDIDATE, not CORE ban |

---

## 6. Wave B CORE batch (Phase 5–6)

1. RULE-RADIUS-SCALE-001 → skill `apply-radius-scale`  
2. RULE-COLOR-RESTRAINT-001 → skill `restrain-decorative-color`  
3. RULE-FORM-FEEDBACK-001 → skill `provide-form-feedback`  
4. RULE-ACTION-001 → skill `rank-actions`

Plus changelog evidence on RULE-SPACE-001 / RULE-COLOR-001.

---

## Definition of Done — Wave B (this pass)

- [x] Material + Atlassian + Polaris forms analyses  
- [x] Synthesis with promotions + holds  
- [x] New CORE rules + universal skills + adapters  
- [x] Validation checklist extended  
- [x] Indexes / plan updated  
