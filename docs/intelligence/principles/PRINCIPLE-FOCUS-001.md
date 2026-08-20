# PRINCIPLE-FOCUS-001 — Visible, Unobscured Focus

```text
Principle:
Every interactive control must show a visible focus indicator that is not
fully obscured, with keyboard focus order matching the dialog/page model.

Problem:
Keyboard and AT users lose their place; hidden focus fails WCAG.

Recommendation:
Provide a clear focus treatment (commonly a distinct focus ring/border).
Ensure sticky headers/footers/overlays do not fully hide focused elements.
In modal dialogs, contain Tab cycles and restore focus on close (see
PRINCIPLE-DIALOG-001).

Why:
Operable interfaces (WCAG) and predictable interaction.

Context:
All pointer+keyboard web UIs; overlays; sticky chrome.

Exceptions:
None for focus visibility on interactive elements. Disabled controls are
non-interactive and typically not focusable.

Evidence:
- ST-001 WCAG 2.2 (2.4.7 Focus Visible; 2.4.11 Focus Not Obscured)
- DS-002 Carbon focus tokens / 3:1 guidance
- DS-005 Primer outline-focus tokens
- ST-002 APG Dialog keyboard notes

Confidence:
High

Category:
06 Accessibility / Focus

StatementClass:
Standard

Maturity:
CORE (formalized as RULE-FOCUS-001, 2026-08-20)

PriorityFloor:
P0
```
