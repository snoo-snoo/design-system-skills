# PRINCIPLE-ACTION-HIERARCHY-001 — Clear Action Hierarchy

```text
Principle:
Present a clear action hierarchy: one primary call-to-action per area,
secondary/default actions for lesser tasks, and danger only for destructive
irreversible confirms.

Problem:
Multiple competing primaries and casual “red” buttons cause hesitation,
mis-clicks, and accidental destructive actions.

Recommendation:
- Use primary appearance for the single most important action in a view/region
  (e.g. Save / Continue / Submit).
- Use default/secondary for ordinary actions; pair subtle/link-style for Cancel
  beside a primary when appropriate.
- Reserve danger for final confirmation of destructive/irreversible actions.
- Use warning appearances for significant change / possible data-loss confirms
  when the system provides that role.
- Prefer explaining blockers with validation over silently disabling the only
  path forward when possible (see CX-006).

Why:
Scannable decisions, error prevention, consistent semantic color of actions.

Context:
Toolbars, forms, dialogs, page headers, empty states with CTAs.

Exceptions:
Independent regions on a dense dashboard may each have one primary.
Marketing landing heroes may use brand-expressive CTAs outside product chrome.

Evidence:
- DS-004 Atlassian Button appearances (primary once per area; danger; warning)
- Aligns with RULE-COLOR-001 role intent (brand/danger/neutral)
- ST-003 Heuristics #4 Consistency, #5 Error prevention

Confidence:
High

Category:
03 Components / Buttons + 04 Patterns

StatementClass:
Practice + System Convention

Maturity:
CORE (formalized as RULE-ACTION-001, Wave B 2026-08-20)

PriorityFloor:
P1 functional clarity / P3 interaction consistency / P0 when danger misused
risks irreversible harm
```
