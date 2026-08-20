# Checklist: consistency

Interaction and pattern consistency across the reviewed UI.

| ID | Check | Severity | Notes |
| --- | --- | --- | --- |
| CON-01 | Same component role uses same interaction model (e.g. all tabs behave as tabs) | P3 | RULE-TABS-001 |
| CON-02 | Focus treatment is recognizable across controls | P3 | RULE-FOCUS-001 |
| CON-03 | Spacing rhythm follows one scale (no random jumps) | P4 | RULE-SPACE-001 |
| CON-04 | Semantic color roles reused for like states (error/success/focus) | P4 | RULE-COLOR-001 |
| CON-05 | Label placement pattern consistent across a form | P3 | RULE-FORM-LABEL-001 |
| CON-06 | Modal dismiss patterns consistent (Esc + visible control) | P3 | RULE-DIALOG-001 |
| CON-07 | No one-off “special” control that breaks platform expectations without docs | P3 | Heuristics #4 |

`fail` on CON-* does not override P0 remediations — fix P0 first.
