# Example Validation Report — Wave A smoke

Illustrative report showing the expected shape after an adapter run. Not a real product audit.

```text
REPORT-ID: VR-20260820-EX01
Target: Sample settings form with confirm modal (synthetic)
SkillsApplied: label-form-fields, build-accessible-modal, ensure-visible-focus
RulesInScope: RULE-FORM-LABEL-001, RULE-DIALOG-001, RULE-FOCUS-001
ModelAdapter: claude
Timestamp: 2026-08-20

CHECKS:
| Checklist | Item ID | Result | Severity | Evidence | Remediation |
| --- | --- | --- | --- | --- | --- |
| wave-a-core | WA-01 | pass | P0 | Focus ring token applied |  |
| wave-a-core | WA-04 | pass | P0 | Labels above inputs |  |
| wave-a-core | WA-05 | pass | P0 | Dialog named + trap + Esc |  |
| wave-a-core | WA-08 | needs-info | P4 | No project spacing tokens provided | Supply token scale |
| accessibility | A11Y-10 | pass | P0 | Esc + Cancel in tab order |  |

SUMMARY:
  PassCount: 4
  FailCount: 0
  Blockers: none
  Verdict: pass-with-warnings

ASSUMPTIONS / NEEDS-INFO:
  - Project spacing/color token files not supplied

FEEDBACK_TO_RULES:
  - none
```
