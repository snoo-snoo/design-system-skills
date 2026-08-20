# SKILL: provide-form-feedback

```text
SKILL: provide-form-feedback

PURPOSE:
Ensure forms give timely, visible, accessible feedback for focus, validation, and progress.

SCOPE / WHEN TO USE:
- Designing or reviewing forms
- Fixing silent validation / toast-only errors
- Pair with label-form-fields and rank-actions

INPUTS:
- Field list + validation rules
- Submit/progress behavior
- Existing error copy

RULES:
1. MUST show visible focus and validation feedback (RULE-FORM-FEEDBACK-001).
2. MUST associate errors/help with fields programmatically and visually.
3. MUST explain what went wrong and how to fix it.
4. SHOULD validate after interaction and/or on submit (avoid premature errors).
5. SHOULD clear errors when inputs become valid.
6. MUST keep persistent labels and not use color-only errors.
7. MUST honor prefers-reduced-motion for animated progress.

CONSTRAINTS / DON'T:
- Don't rely on distant toasts alone for field errors.
- Don't disable submit without explanation (CX-006).

DECISION LOGIC: (P0–P7)
Accessible error association and clarity are P0/P1 over aesthetic minimalism.

ACCESSIBILITY:
Align with WCAG error identification/suggestion direction; aria-describedby patterns.

OUTPUT REQUIREMENTS:
- Feedback plan per field + form-level
- Error copy samples
- AT association notes

EDGE CASES:
- OTP live validation; async uniqueness checks; offline batch

VALIDATION / SELF-REVIEW:
- [ ] Field errors in context + associated
- [ ] Copy is specific and actionable
- [ ] Progress/focus feedback visible without motion-only cues
- [ ] Labels remain persistent

RELATED SKILLS: label-form-fields, ensure-visible-focus, rank-actions
SOURCE RULES: RULE-FORM-FEEDBACK-001, RULE-FORM-LABEL-001, RULE-FOCUS-001
```
