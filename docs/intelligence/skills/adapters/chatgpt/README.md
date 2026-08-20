# ChatGPT Adapter Profile

```text
ADAPTER PROFILE: chatgpt
MODEL family: OpenAI ChatGPT
```

## Prompting style

- Use numbered steps and checklists the user can paste into reviews.
- Offer an optional JSON block for machine-readable validation results.
- Keep explanations plain; link claims to RULE-IDs.
- When using structured output modes, map fields to the Validation Report schema.

## Tool hints

- If browsing/code tools are available, verify against live docs/code.
- Otherwise label inferences as assumptions.

## Output shaping

```text
## Summary
## Step-by-step changes
## Self-review checklist
## Validation report
### Optional JSON
{ "verdict": "...", "blockers": [], "warnings": [], "needs_info": [] }
## Assumptions
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
