# Checklist: wave-a-core

Default checklist for any Wave A CORE skill/adapter output.

Mark each item: `pass` | `fail` | `n/a` | `needs-info`.

## P0 — Accessibility & operable UI

| ID | Check | Related rules |
| --- | --- | --- |
| WA-01 | Interactive controls have a visible focus indicator | RULE-FOCUS-001 |
| WA-02 | Focused elements are not fully obscured by sticky/overlay chrome | RULE-FOCUS-001 |
| WA-03 | Applicable pointer targets meet WCAG minimum target size (or documented exception) | RULE-TOUCH-001 |
| WA-04 | Data-entry fields have persistent visible labels (not placeholder-only) | RULE-FORM-LABEL-001 |
| WA-05 | True modals are named, focus-trapped, Esc-dismissible, restore focus | RULE-DIALOG-001 |
| WA-06 | Tabs use correct roles/selection and arrow-key list navigation when tabs are present | RULE-TABS-001 |
| WA-07 | Text/critical UI contrast not knowingly broken; color roles used for product UI | RULE-COLOR-001 |

## P4 — Design-system consistency

| ID | Check | Related rules |
| --- | --- | --- |
| WA-08 | Spacing uses project tokens / discrete scale (no new magic numbers) | RULE-SPACE-001 |
| WA-09 | Product colors use semantic tokens/themes (no raw hex sprawl) | RULE-COLOR-001 |

## Meta

| ID | Check |
| --- | --- |
| WA-10 | Output stayed within one atomic skill (no silent mega-prompt expansion) |
| WA-11 | Open contradictions not “resolved” by inventing consensus |
| WA-12 | Assumptions / needs-info explicitly listed |

## Scoring

- Any WA-01…WA-07 `fail` → overall **fail**
- WA-08…WA-09 `fail` → warning (system bar) unless project treats P4 as gate
- WA-10…WA-12 `fail` → process warning; fix before trusting the report
