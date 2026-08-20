# Validation Loop

Repeatable loop after any Universal Skill or Model Adapter run.

```text
1. APPLY SKILL / ADAPTER
        ↓
2. SKILL SELF-REVIEW
   (checklist embedded in Universal Skill)
        ↓
3. RUN CHECKLISTS
   always: wave-a-core
   plus: accessibility / consistency / ux / design-system as scoped
        ↓
4. CLASSIFY RESULTS
   pass | fail | n/a | needs-info
   attach Severity P0–P7
        ↓
5. REMEDIATE
   fix Must-fix (P0–P1) before optional polish
        ↓
6. RE-RUN FAILED CHECKS
        ↓
7. EMIT VALIDATION REPORT
   docs/intelligence/validation/reports/_template.md
        ↓
8. OPTIONAL RULE FEEDBACK
   route durable learnings to research / contradiction log
   (do not silently mutate CORE rules)
```

## Verdict rules

| Condition | Verdict |
| --- | --- |
| Any P0 `fail` | `fail` |
| No P0 fail; any P1–P3 fail | `pass-with-warnings` (or `fail` if release bar requires it) |
| Only P4–P7 fails / n/a | `pass-with-warnings` or `pass` per project bar |
| Missing critical context | `needs-info` items required; do not fake pass |

## Minimum bar (this repo / Wave A)

- Ship / accept only if **no P0 fails** on `wave-a-core`.
- Adapter runs must include Validation Report summary in the model output.

## Application wiring (conceptual)

For UI generation, UX review, or design audit apps:

1. Select skills (atomic; one task each).
2. Select adapter profile for the host model.
3. Execute skill.
4. Execute this loop.
5. Persist report; block merge/publish on P0 fail.
