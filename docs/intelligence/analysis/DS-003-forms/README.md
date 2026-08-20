# DS-003 Forms — Polaris Text Field / Inline Error (Wave B)

**Status:** analyzed (2026-08-20)  
**Pages:** Polaris Text field usage · Inline error component · Error messages content guidelines

## Claim inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| POL-F1 | Validate after the user finishes interacting with a field (not before) | Practice | High |
| POL-F2 | Show field errors in context (inline); associate with the field (`aria-describedby` / fieldID) | Practice + A11y | High |
| POL-F3 | Error copy is brief, sentence case, explains what went wrong and how to fix | Content Practice | High |
| POL-F4 | Remove the error as soon as the input becomes valid | Practice | High |
| POL-F5 | Help text and errors are exposed to AT with the label | A11y / Standard-aligned | High |
| POL-F6 | Labels should make the expected input obvious; mark optional when needed | Practice | High |

## Principle links

- Promotes PRINCIPLE-FORM-FEEDBACK-001 → CORE  
- Reinforces RULE-FORM-LABEL-001  
- Aligns with ST-003 Heuristic #1 (system status) and WCAG error identification/suggestion direction

## Notes

- Commerce/admin context — timing “after blur” is a strong default, not the only valid strategy (submit-time validation still OK if errors are clear).
