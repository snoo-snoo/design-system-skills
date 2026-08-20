# Checklist: accessibility

Use with focus, targets, labels, dialogs, tabs, and contrast-sensitive color work.

| ID | Check | Severity | Rules |
| --- | --- | --- | --- |
| A11Y-01 | Visible focus on all focusable controls | P0 | RULE-FOCUS-001 |
| A11Y-02 | No `outline:none` / equivalent without replacement | P0 | RULE-FOCUS-001 |
| A11Y-03 | Focus not fully obscured | P0 | RULE-FOCUS-001 |
| A11Y-04 | Hit areas meet minimum target size | P0 | RULE-TOUCH-001 |
| A11Y-05 | Primary mobile actions comfortably tappable (SHOULD) | P1 | RULE-TOUCH-001 |
| A11Y-06 | Persistent visible labels on fields | P0 | RULE-FORM-LABEL-001 |
| A11Y-07 | Placeholder not used as only label | P0 | RULE-FORM-LABEL-001 |
| A11Y-08 | Modal accessible name present | P0 | RULE-DIALOG-001 |
| A11Y-09 | Modal focus in on open / restore on close | P0 | RULE-DIALOG-001 |
| A11Y-10 | Modal Tab cycle + Esc + visible dismiss | P0 | RULE-DIALOG-001 |
| A11Y-11 | Background inert while modal open | P0 | RULE-DIALOG-001 |
| A11Y-12 | Tabs: tablist/tab/tabpanel + single selection | P0 | RULE-TABS-001 |
| A11Y-13 | Tabs: arrow keys in list; Tab enters panel | P0 | RULE-TABS-001 |
| A11Y-14 | Contrast for text / required non-text UI addressed | P0 | RULE-COLOR-001 |
| A11Y-15 | Disabled-contrast claims not elevated without CX-002 resolution | P0 process | CX-002 |

Mark `n/a` when the component type is absent from the target.
