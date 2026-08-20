# RULE-BORDER-RESTRAINT-001 — Prefer Space Over Decorative Borders

```text
RULE-BORDER-RESTRAINT-001
Name: Prefer Space Over Decorative Borders
Category: 02 Layout + 01 Foundations / Spacing
Principle: PRINCIPLE-BORDER-RESTRAINT-001
Recommendation:
  SHOULD create layout hierarchy primarily with spacing, proximity, and
  typography — not dense decorative borders/dividers.
  MUST NOT remove borders required for affordance, focus indication, or contrast
  (inputs, tables when needed, focus rings, editable regions).
  MAY use design-system divider components sparingly when separation is necessary.
Reason:
  Excess borders add noise and compete with content.
Context:
  Dashboards, settings, content layouts, card stacks.
Exceptions:
  Form controls; focus indicators; data tables; high-density tools; low-contrast
  media needing edge definition; required DS divider patterns.
Anti-pattern:
  Boxing every block with 1px borders “for structure.”
  Stripping input/focus borders for a “borderless” aesthetic (P0 fail).
Evidence:
  - VID-SAMPLE-006
  - RULE-SPACE-001 (proximity/hierarchy)
  - CX-005 noted exceptions
  - Related: RULE-CARD-SURFACE-001
Confidence: Medium–High
Maturity: CORE
Related Rules: RULE-SPACE-001, RULE-FOCUS-001, RULE-CARD-SURFACE-001
PriorityFloor: P5 craft / P2 hierarchy — never overrides P0 focus/contrast
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE by product decision (CANDIDATE → prod)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| P0 protections | ✅ |
| Anti-pattern | ✅ |
