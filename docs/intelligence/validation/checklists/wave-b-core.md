# Checklist: wave-b-core

Default checklist for Wave B CORE skill/adapter output (actions, form feedback, radius scale, color restraint). Run **in addition to** `wave-a-core.md` when Wave B skills are used.

Mark each item: `pass` | `fail` | `n/a` | `needs-info`.

## Actions & feedback

| ID | Check | Related rules |
| --- | --- | --- |
| WB-01 | ≤1 primary CTA per view/region | RULE-ACTION-001 |
| WB-02 | Danger styling reserved for destructive irreversible confirms | RULE-ACTION-001 |
| WB-03 | Field errors are in context and associated with controls | RULE-FORM-FEEDBACK-001 |
| WB-04 | Error copy explains problem + fix; not color-only | RULE-FORM-FEEDBACK-001 |
| WB-05 | Progress/focus feedback is visible without motion-only cues | RULE-FORM-FEEDBACK-001 |
| WB-06 | Unexplained disabled primary avoided when validation can explain blockers | RULE-ACTION-001 / CX-006 |

## Foundations (Wave B promotions)

| ID | Check | Related rules |
| --- | --- | --- |
| WB-07 | Radii map to semantic shape/radius scale (no magic radii) | RULE-RADIUS-SCALE-001 |
| WB-08 | Decorative accents not used for semantic status/action meaning | RULE-COLOR-RESTRAINT-001 |

## Scoring

- Any WB-01…WB-05 `fail` on an applicable UI → treat as **fail** for Wave B bar (WB-02/03/04 are P0-adjacent when destructive or error paths exist)
- WB-06 `fail` → warning unless it blocks task completion with no explanation → **fail**
- WB-07…WB-08 `fail` → P4 warnings unless project gates system consistency
