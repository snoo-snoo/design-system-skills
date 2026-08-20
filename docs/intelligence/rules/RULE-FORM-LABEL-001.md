# RULE-FORM-LABEL-001 — Persistent Visible Field Labels

```text
RULE-FORM-LABEL-001
Name: Persistent Visible Field Labels
Category: 04 Patterns / Forms + 07 Content + 06 Accessibility
Principle: PRINCIPLE-FORM-LABEL-001
Recommendation:
  MUST provide a persistent, visible label for each form field (typically
  above or beside the control in reading order).
  MUST NOT rely on placeholder-only labeling for required or data-entry fields.
  SHOULD use placeholder/hint text only for format examples, not as the label.
  SHOULD prefer persistent labels over floating-label-as-default patterns.
Reason:
  Missing or disappearing labels increase errors, hurt zoom/AT use, and
  fail clear labeling expectations (WCAG Labels or Instructions).
Context:
  Settings, onboarding, checkout, fintech, and general data-entry forms.
Exceptions:
  Severely constrained search fields with a visible nearby legend.
  Specialized, tested patterns that still expose accessible names persistently
  to AT — document as exceptions, not the product default.
  Brand products may ship floating labels; they remain non-default here
  (CX-003 resolution).
Anti-pattern:
  Placeholder-as-only-label.
  Floating label that vanishes or becomes hard to read while filling.
  Icon-only fields without accessible name and visible text label.
Evidence:
  - ST-001 WCAG 2.2 SC 3.3.2 Labels or Instructions (directional)
  - CX-003 resolution vs VID-SAMPLE-004 floating-label tip
  - Community a11y critique corpus on floating labels / placeholder labels
Confidence: High
Maturity: CORE
Related Rules: RULE-FOCUS-001, RULE-TOUCH-001, RULE-FORM-FEEDBACK (future)
PriorityFloor: P0
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE; CX-003 default = persistent labels (Wave-A)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-FORM-LABEL-001 |
| Source IDs | ST-001, VID-SAMPLE-004 (conflict source) |
| Normalized from | PRINCIPLE-FORM-LABEL-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Contradiction | CX-003 resolved for defaults |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ Standard pressure + conflict resolution |
| Accessibility-compatible | ✅ |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ CX-003 |
