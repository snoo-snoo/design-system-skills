# PRINCIPLE-BORDER-RESTRAINT-001 — Prefer Space Over Decorative Borders

```text
Principle:
Create layout hierarchy primarily with spacing (and subtle surface/type
shifts), not with dense borders and divider lines.

Problem:
Excess borders/dividers add noise and make interfaces feel like spreadsheets.

Recommendation:
Default to whitespace, proximity, and typography for grouping. Add borders
when they provide necessary structure, affordance, or accessibility contrast
(e.g. inputs, tables, focus, editable regions, required separation on busy
backgrounds).

Why:
Cleaner hierarchy, less visual competition, stronger content focus.

Context:
Product UI dashboards, settings, content layouts, card stacks.

Exceptions:
- Form controls and focus indicators (often require visible edges)
- Data tables / spreadsheets (borders can aid scanning)
- High-density enterprise tools where separators prevent misreads
- Low-contrast media where a border restores target perception
- Explicit design-system divider components used sparingly

Evidence:
- VID-SAMPLE-006
- PRINCIPLE-SPACE-001 (Carbon spacing / proximity)
- PRINCIPLE-CARD-SURFACE-001 (related chrome restraint)
- Comment consensus: whitespace + subtle color can replace lines

Confidence:
Medium–High

Category:
02 Layout + 01 Foundations / Spacing

StatementClass:
Practice

Maturity:
CORE (formalized as RULE-BORDER-RESTRAINT-001, 2026-08-20 — prod promotion)

PriorityFloor:
P5 craft / P2 hierarchy — never remove borders required for P0 focus/contrast
```
