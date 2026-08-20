# RULE-DIALOG-001 — Modal Dialog Focus & Naming

```text
RULE-DIALOG-001
Name: Modal Dialog Focus & Naming
Category: 03 Components / Modals + 06 Accessibility
Principle: PRINCIPLE-DIALOG-001
Recommendation:
  MUST name the dialog (prefer aria-labelledby to a visible title; else aria-label).
  MUST treat true modals as modal for everyone (background not operable).
  MUST move focus into the dialog on open and restore focus to the invoker on close
  (unless a documented workflow exception applies).
  MUST trap Tab / Shift+Tab inside the modal while open.
  MUST support Escape to dismiss and include a visible close/cancel control
  in the tab order.
  SHOULD choose initial focus based on content risk (destructive confirms vs
  simple notices).
Reason:
  Broken modals strand keyboard/AT users and leave “inert-looking” backgrounds
  still interactive — fails operable/understandable expectations.
Context:
  Web modal dialogs, confirmations, multi-step overlays.
Exceptions:
  Non-modal dialogs (different pattern).
  alertdialog special cases per APG.
  Native <dialog> (or equivalent) implementations that meet the same behaviors.
Anti-pattern:
  Div overlay without dialog semantics or accessible name.
  Focus left on the trigger while the modal is open.
  Background still tabbable; no Esc handler; focus lost on close.
Evidence:
  - ST-002 APG Dialog (Modal) Pattern
  - ST-001 focus-related success criteria
  - ST-003 Heuristics #1 System status, #3 User control
Confidence: High
Maturity: CORE
Related Rules: RULE-FOCUS-001, RULE-TABS-001
PriorityFloor: P0
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-DIALOG-001 (Wave-A APG consensus)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-DIALOG-001 |
| Source IDs | ST-002, ST-001, ST-003 |
| Normalized from | PRINCIPLE-DIALOG-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ APG + WCAG + Heuristics |
| Accessibility-compatible | ✅ |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ non-modal / native dialog exceptions |
