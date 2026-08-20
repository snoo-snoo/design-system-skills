# Grok Adapter Profile

```text
ADAPTER PROFILE: grok
MODEL family: xAI Grok
```

## Prompting style

- Be direct and terse. Lead with the decision, then evidence.
- Use MUST / SHOULD / MAY language exactly as in the Universal Skill.
- Call out anti-patterns bluntly; no soft-pedaling P0 failures.
- Avoid decorative filler and marketing tone.

## Tool hints

- Prefer concrete, testable checks (focus ring present? hit area ≥ minimum?).
- If context is missing, list blockers first.

## Output shaping

```text
## Verdict
## Must-fix
## Should-fix
## Self-review
## Validation (P0 blockers first)
## Gaps
```

## Validation hook

Always run:

- `validation/checklists/wave-a-core.md`
- Plus skill-relevant checklists (see each skill adapter)

## Skill adapters

| Universal Skill | Adapter |
| --- | --- |
| ensure-visible-focus | [ensure-visible-focus.md](ensure-visible-focus.md) |
| size-touch-targets | [size-touch-targets.md](size-touch-targets.md) |
| label-form-fields | [label-form-fields.md](label-form-fields.md) |
| build-accessible-modal | [build-accessible-modal.md](build-accessible-modal.md) |
| build-accessible-tabs | [build-accessible-tabs.md](build-accessible-tabs.md) |
| apply-spacing-scale | [apply-spacing-scale.md](apply-spacing-scale.md) |
| apply-semantic-color | [apply-semantic-color.md](apply-semantic-color.md) |
