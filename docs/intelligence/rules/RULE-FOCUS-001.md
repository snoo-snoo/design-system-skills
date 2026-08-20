# RULE-FOCUS-001 — Visible, Unobscured Focus

```text
RULE-FOCUS-001
Name: Visible, Unobscured Focus
Category: 06 Accessibility / Focus
Principle: PRINCIPLE-FOCUS-001
Recommendation:
  MUST show a visible focus indicator on every interactive control that can
  receive keyboard focus.
  MUST ensure focused elements are not fully obscured by sticky chrome,
  drawers, or overlays (WCAG Focus Not Obscured).
  SHOULD use a distinct focus treatment (commonly a focus ring/border with
  sufficient contrast against adjacent colors).
  MUST keep focus order coherent with the page/dialog interaction model.
Reason:
  Keyboard and assistive-technology users need a reliable place indicator;
  hidden focus fails WCAG and traps users.
Context:
  All pointer+keyboard web UIs; overlays; sticky headers/footers; modal dialogs
  (also see RULE-DIALOG-001).
Exceptions:
  Disabled non-interactive controls are typically not focusable.
  Purely presentational elements must not be focusable.
Anti-pattern:
  outline: none / ring-0 with no replacement focus style.
  Focus landing behind sticky bars or modal backdrops.
  Tab order that skips into inert background content.
Evidence:
  - ST-001 WCAG 2.2 SC 2.4.7 Focus Visible; 2.4.11 Focus Not Obscured
  - DS-002 Carbon focus tokens / contrast guidance
  - DS-005 Primer outline-focus tokens
  - ST-002 APG Dialog keyboard notes
Confidence: High
Maturity: CORE
Related Rules: RULE-DIALOG-001, RULE-TOUCH-001
PriorityFloor: P0
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-FOCUS-001 (Wave-A synthesis)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-FOCUS-001 |
| Source IDs | ST-001, ST-002, DS-002, DS-005 |
| Normalized from | PRINCIPLE-FOCUS-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix (Standard + DS) | ✅ |
| Accessibility-compatible | ✅ (is P0) |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ none critical |
