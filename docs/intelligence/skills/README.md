# Skills Index — Phases 6–7

## Universal Skills (Phase 6) — Source of Truth

| Skill | Task | Source Rules |
| --- | --- | --- |
| [ensure-visible-focus](universal/ensure-visible-focus.md) | Audit/fix focus visibility | RULE-FOCUS-001 |
| [size-touch-targets](universal/size-touch-targets.md) | Enforce adequate hit areas | RULE-TOUCH-001 |
| [label-form-fields](universal/label-form-fields.md) | Persistent field labels | RULE-FORM-LABEL-001 |
| [build-accessible-modal](universal/build-accessible-modal.md) | Modal dialog a11y behavior | RULE-DIALOG-001 |
| [build-accessible-tabs](universal/build-accessible-tabs.md) | Tabs structure & keyboard | RULE-TABS-001 |
| [apply-spacing-scale](universal/apply-spacing-scale.md) | Tokenized spacing | RULE-SPACE-001 |
| [apply-semantic-color](universal/apply-semantic-color.md) | Semantic color tokens | RULE-COLOR-001 |

## Model Adapters (Phase 7)

Thin wrappers — **do not fork** Universal Skills.

| Model | Entry |
| --- | --- |
| Claude | [adapters/claude/](adapters/claude/) |
| Grok | [adapters/grok/](adapters/grok/) |
| ChatGPT | [adapters/chatgpt/](adapters/chatgpt/) |

Contract: [adapters/contract.md](adapters/contract.md) · Invoke: [adapters/invoke-template.md](adapters/invoke-template.md)

## Validation (Phase 8)

After every skill/adapter run: [../validation/README.md](../validation/README.md)

## Atomicity

One skill = one task. Adapters change tone/shape only.
