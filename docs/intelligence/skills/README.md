# Universal Skills Index — Phase 6

Model-independent AI Design Skills. **Source of Truth.** Generated only from CORE Canonical Rules.

| Skill | Task | Source Rules |
| --- | --- | --- |
| [ensure-visible-focus](universal/ensure-visible-focus.md) | Audit/fix focus visibility | RULE-FOCUS-001 |
| [size-touch-targets](universal/size-touch-targets.md) | Enforce adequate hit areas | RULE-TOUCH-001 |
| [label-form-fields](universal/label-form-fields.md) | Persistent field labels | RULE-FORM-LABEL-001 |
| [build-accessible-modal](universal/build-accessible-modal.md) | Modal dialog a11y behavior | RULE-DIALOG-001 |
| [build-accessible-tabs](universal/build-accessible-tabs.md) | Tabs structure & keyboard | RULE-TABS-001 |
| [apply-spacing-scale](universal/apply-spacing-scale.md) | Tokenized spacing | RULE-SPACE-001 |
| [apply-semantic-color](universal/apply-semantic-color.md) | Semantic color tokens | RULE-COLOR-001 |

## Atomicity

One skill = one task. Do not merge into “make the whole UI good.”

## Adapters

Phase 7: wrap these Universal Skills in model-specific adapters under `adapters/` — do not fork rule content.
