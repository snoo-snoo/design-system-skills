# RULE-FORM-FEEDBACK-001 — Visible Form Interaction Feedback

```text
RULE-FORM-FEEDBACK-001
Name: Visible Form Interaction Feedback
Category: 04 Patterns / Forms + 05 UX + 06 Accessibility
Principle: PRINCIPLE-FORM-FEEDBACK-001
Recommendation:
  MUST provide timely visible feedback for focus, validation errors, and
  in-progress submission states — not motion alone.
  MUST associate field-level error/help text with the control (e.g.
  aria-describedby) and keep errors in visual context of the field.
  SHOULD validate after the user finishes interacting with a field and/or on
  submit; avoid yelling errors before interaction unless format is tightly
  constrained.
  MUST explain what went wrong and how to fix it in brief, specific copy.
  SHOULD clear field errors as soon as the input becomes valid.
  MUST honor prefers-reduced-motion for progress/animation feedback.
  MUST keep persistent labels (RULE-FORM-LABEL-001) and visible focus
  (RULE-FOCUS-001) while providing feedback.
Reason:
  Silent forms raise uncertainty and error rates; AT users need programmatically
  associated messages (system status + accessible descriptions).
Context:
  Settings, onboarding, checkout, fintech, admin forms.
Exceptions:
  Offline/batch validation — communicate pending state explicitly.
Anti-pattern:
  Errors only in a distant toast with no field association.
  Placeholder-only error hints; color-only error indication.
  Blocking progress with a disabled submit and no explanation (see CX-006).
Evidence:
  - ST-003 Heuristic #1 Visibility of system status
  - DS-003 Polaris Text field / Inline error (+ content error guidelines)
  - ST-001 WCAG error identification / suggestion (directional)
  - VID-SAMPLE-004 (supporting Practice)
  - RULE-FORM-LABEL-001, RULE-FOCUS-001
Confidence: High
Maturity: CORE
Related Rules: RULE-FORM-LABEL-001, RULE-FOCUS-001, RULE-ACTION-001
PriorityFloor: P1 clarity / P0 when errors or status are required to proceed safely
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE in Wave B (Polaris forms + heuristics)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Evidence mix | ✅ |
| A11y compatible | ✅ |
| Anti-pattern | ✅ |
