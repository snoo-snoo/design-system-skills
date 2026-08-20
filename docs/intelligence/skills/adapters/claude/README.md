# Claude Adapter Profile

```text
ADAPTER PROFILE: claude
MODEL family: Anthropic Claude
```

## Prompting style

- Prefer clear section headings and short bullet proofs over long essays.
- Treat Universal Skill RULES as policy; quote rule IDs when making MUST claims.
- When uncertain, say `needs-info` instead of inventing tokens or a11y exceptions.
- Favor structured final answers: Findings → Changes → Self-review → Validation.

## Tool hints

- If code tools exist: inspect real CSS/components before asserting focus/target sizes.
- If only prose: mark assumptions explicitly.

## Output shaping

```text
## Findings
## Proposed changes
## Self-review (skill checklist)
## Validation report (wave-a-core + relevant checklists)
## Assumptions / needs-info
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
| apply-radius-scale | [apply-radius-scale](apply-radius-scale.md) |
| restrain-decorative-color | [restrain-decorative-color](restrain-decorative-color.md) |
| provide-form-feedback | [provide-form-feedback](provide-form-feedback.md) |
| rank-actions | [rank-actions](rank-actions.md) |
