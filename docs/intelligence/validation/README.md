# Validation — Phase 8

Validation Loop for outputs from Universal Skills and Model Adapters.

| Artifact | Purpose |
| --- | --- |
| [loop.md](loop.md) | Process: generate → self-review → checklist → remediate → report |
| [checklists/](checklists/) | Reusable review checklists |
| [reports/_template.md](reports/_template.md) | Validation report template |
| [../schemas/validation-report.md](../schemas/validation-report.md) | Schema |

## Checklists

| ID | File | Use when |
| --- | --- | --- |
| wave-a-core | [checklists/wave-a-core.md](checklists/wave-a-core.md) | Any Wave A CORE skill/adapter run (default) |
| wave-b-core | [checklists/wave-b-core.md](checklists/wave-b-core.md) | Wave B skills (actions, form feedback, radius, color restraint) |
| accessibility | [checklists/accessibility.md](checklists/accessibility.md) | Focus, targets, labels, dialogs, tabs, contrast |
| consistency | [checklists/consistency.md](checklists/consistency.md) | Interaction & pattern consistency |
| ux | [checklists/ux.md](checklists/ux.md) | Clarity, feedback, error prevention |
| design-system | [checklists/design-system.md](checklists/design-system.md) | Tokens, themes, API parity with system |

## Hard rules

1. P0 failures → verdict `fail` (block ship).
2. Do not invent consensus to pass a check.
3. Open contradictions (CX-*) stay open; document `needs-info` or scoped exception.
4. Feedback that may change rules goes back to research — do not silently edit CORE rules from a single run.
