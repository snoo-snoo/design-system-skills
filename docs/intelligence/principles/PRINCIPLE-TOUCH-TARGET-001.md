# PRINCIPLE-TOUCH-TARGET-001 — Adequate Pointer Targets

```text
Principle:
Interactive targets must be large enough for reliable pointer/touch use.

Problem:
Small controls cause mis-taps, errors, and exclusion—especially on mobile.

Recommendation:
Size hit areas to meet accessibility minimums (WCAG 2.2 Target Size) and
prefer comfortable thumb-friendly targets for primary mobile actions.
Padding can enlarge hit area without enlarging visuals.

Why:
Error prevention + operable UI (P0).

Context:
All pointer UIs; critical for mobile fintech/forms (VID-SAMPLE-004).

Exceptions:
Inline text links have specific WCAG exception paths—prefer larger controls
for primary actions anyway.

Evidence:
- ST-001 WCAG 2.2 Success Criterion 2.5.8 Target Size (Minimum)
- VID-SAMPLE-004 Revolut “Touch Targets” principle
- DS-005 Primer control size tokens (practical sizing system)

Confidence:
High

Category:
01 Sizing / 06 Accessibility / 03 Components

StatementClass:
Standard (+ Practice)

Maturity:
CORE (formalized as RULE-TOUCH-001, 2026-08-20)

PriorityFloor:
P0
```
