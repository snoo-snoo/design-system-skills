# PRINCIPLE-DIALOG-001 — Modal Dialog Focus & Naming

```text
Principle:
Modal dialogs must be named, modal for everyone, focus-trapped, Esc-dismissible,
and restore focus on close.

Problem:
Broken modals trap or strand keyboard/AT users and expose inert-looking but
still interactive backgrounds.

Recommendation:
- Container role `dialog` with `aria-modal="true"` only when truly modal for all users
- Accessible name via `aria-labelledby` (preferred) or `aria-label`
- On open: move focus into dialog (choose initial focus by content/risk)
- Tab / Shift+Tab cycle inside dialog
- Escape closes; include a visible close/cancel control in tab order
- On close: return focus to invoker (unless workflow exception)

Why:
Matches APG Dialog (Modal) pattern and WCAG operable/understandable expectations.

Context:
Web modal dialogs, confirmations, multi-step overlays.

Exceptions:
Non-modal dialogs (different pattern); alertdialog special cases; native
`<dialog>` implementations that meet equivalent behaviors.

Evidence:
- ST-002 APG Dialog (Modal) Pattern
- ST-001 focus-related SC
- ST-003 Heuristics #3 User control, #1 System status (overlay)

Confidence:
High

Category:
03 Components / Modals + 06 Accessibility

StatementClass:
Standard-adjacent Pattern Spec

Maturity:
CORE (formalized as RULE-DIALOG-001, 2026-08-20; APG + WCAG consensus)

PriorityFloor:
P0
```
