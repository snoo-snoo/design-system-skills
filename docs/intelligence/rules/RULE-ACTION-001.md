# RULE-ACTION-001 — Clear Action Hierarchy

```text
RULE-ACTION-001
Name: Clear Action Hierarchy
Category: 03 Components / Buttons + 04 Patterns
Principle: PRINCIPLE-ACTION-HIERARCHY-001
Recommendation:
  MUST present a clear visual hierarchy of actions in each view/region.
  SHOULD use exactly one primary CTA per area for the most important action
  (not every screen requires a primary).
  SHOULD use default/secondary styles for ordinary actions; use subtle/link
  styles for Cancel beside a primary when appropriate.
  MUST reserve danger styling for final confirmation of destructive,
  irreversible actions.
  SHOULD use warning styling (when available) for significant change /
  possible data-loss confirms.
  SHOULD prefer validation messaging over an unexplained disabled primary
  submit when users need a path forward (CX-006).
Reason:
  Competing primaries and casual destructive styling increase errors and
  decision friction.
Context:
  Forms, dialogs, headers, toolbars, empty states.
Exceptions:
  Independent dashboard regions may each have one primary.
  Marketing heroes outside product chrome.
Anti-pattern:
  Three primary buttons in one toolbar.
  Red/danger styling on non-destructive actions for “emphasis.”
  Disabled Save with no error text explaining why.
Evidence:
  - DS-004 Atlassian Button appearances (primary once per area; danger; warning)
  - RULE-COLOR-001 / RULE-COLOR-RESTRAINT-001 (semantic action color)
  - ST-003 Heuristics #4, #5
Confidence: High
Maturity: CORE
Related Rules: RULE-COLOR-001, RULE-COLOR-RESTRAINT-001, RULE-FORM-FEEDBACK-001, RULE-DIALOG-001
PriorityFloor: P1 / P3; P0 when danger misuse risks irreversible harm
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Added CORE in Wave B from Atlassian button guidance
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Evidence | ✅ strong DS + heuristics (Wave B); additional DS button pages welcome later |
| A11y compatible | ✅ |
| Anti-pattern | ✅ |
| Conflicts documented | ✅ CX-006 |
