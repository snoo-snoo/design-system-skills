# PRINCIPLE-SPACE-001 — Tokenized Spacing Scale

```text
Principle:
Space the UI using a discrete spacing scale (tokens), not arbitrary px values.

Problem:
Ad-hoc margins/paddings create inconsistent rhythm and weak hierarchy.

Recommendation:
Apply spacing tokens (commonly 2/4/8-based) for component-internal and
layout spacing. Prefer parent layout/stack gaps over scattering margins
inside every child. At breakpoints, jump token steps rather than inventing
off-scale values.

Why:
Predictable rhythm, easier theming, clearer perceived relationships
(proximity) and hierarchy (surrounding space).

Context:
Product UI layout and component construction (web/admin/enterprise and
general product surfaces).

Exceptions:
Rare one-off optical adjustments; percentage-based splits for page structure;
third-party embeds. Document exceptions explicitly.

Evidence:
- DS-002 Carbon Spacing overview (scale + designing-with-space + FAQ)
- DS-005 Primer size/stack tokens
- (Supporting) DS-003 Card padding token usage

Confidence:
High

Category:
01 Foundations / Spacing

StatementClass:
System Convention

Maturity:
CORE (formalized as RULE-SPACE-001, 2026-08-20; Carbon + Primer consensus)

PriorityFloor:
P4
```
