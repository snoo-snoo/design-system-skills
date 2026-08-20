# Checklist: craft-core

Checklist for craft/composition CORE skills promoted from former CANDIDATE/EXPERIMENTAL principles. Run with `wave-a-core` (+ `wave-b-core` when relevant).

Mark: `pass` | `fail` | `n/a` | `needs-info`.

| ID | Check | Rule |
| --- | --- | --- |
| CR-01 | Nested rounded surfaces address concentricity; radii on scale | RULE-NESTED-RADIUS-001 |
| CR-02 | Multi-line product text is start-aligned unless short/intentional center | RULE-TEXT-ALIGN-001 |
| CR-03 | Decorative border density restrained; P0 input/focus/table edges kept | RULE-BORDER-RESTRAINT-001 |
| CR-04 | Design props map to implementation API (or marked non-API) | RULE-COMPONENT-API-001 |
| CR-05 | Card chrome used intentionally; removals preserve contrast/affordance | RULE-CARD-SURFACE-001 |

## Scoring

- CR-03 / CR-05 P0 contrast or focus regressions → **fail**
- Other CR fails → warnings for craft bar (project may gate them)
