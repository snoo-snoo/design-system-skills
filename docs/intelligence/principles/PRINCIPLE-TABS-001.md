# PRINCIPLE-TABS-001 — Tabs Structure & Keyboard

```text
Principle:
Tabs expose one panel at a time with correct roles, selection state, and
arrow-key navigation in the tab list.

Problem:
Fake tabs (links/buttons without tab semantics) break AT navigation and
keyboard expectations.

Recommendation:
- Roles: `tablist` > `tab` + associated `tabpanel`
- Only one `aria-selected="true"` tab; panels labelled by their tab
- `aria-controls` / `aria-labelledby` associations
- Arrow keys move across tabs; Tab key moves into the active panel/page sequence
- Prefer automatic activation when panels are fast/preloaded; otherwise manual
  activation (Space/Enter) per APG guidance
- Set `aria-orientation="vertical"` when vertical

Why:
Predictable keyboard UX and correct AT structure (APG Tabs Pattern).

Context:
In-page tabbed content (not primary site navigation unless designed as tabs).

Exceptions:
Carousel-like patterns; segmented controls that are not tabpanels; native
select on small screens as progressive enhancement (document as alternate pattern).

Evidence:
- ST-002 APG Tabs Pattern
- ST-003 Heuristics #4 Consistency, #6 Recognition over recall

Confidence:
High

Category:
03 Components / Tabs + 06 Accessibility

StatementClass:
Standard-adjacent Pattern Spec

Maturity:
CANDIDATE

PriorityFloor:
P0 for semantics/keyboard; P3 for visual selection styling
```
