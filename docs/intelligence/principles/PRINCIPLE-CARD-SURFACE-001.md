# PRINCIPLE-CARD-SURFACE-001 — Card Chrome Only When Needed

```text
Principle:
Do not wrap every content block in a filled card background by default;
add surface chrome when it improves grouping, affordance, or contrast.

Problem:
Ubiquitous card fills create visual noise and reduce white space; removing
needed surfaces can harm readability and target separation.

Recommendation:
Prefer content + spacing/divider hierarchy first. Use filled/bordered cards
when the group needs clear containment, interactivity affordance, or contrast
against a busy background.

Why:
More focus on content; less redundant chrome — when contrast remains adequate.

Context:
Media/content feeds, marketing-influenced product lists, image-forward UIs.

Exceptions:
Dense enterprise tables/lists needing row/card separation; low-contrast media;
accessible touch grouping; forms inside elevated surfaces.

Evidence:
- VID-SAMPLE-003 (educator tip + brand citations)
- Comment conflict on a11y/readability
- PRINCIPLE-SPACE-001 (proximity can replace chrome)

Confidence:
Medium

Category:
03 Components / Cards

StatementClass:
Practice

Maturity:
CORE (formalized as RULE-CARD-SURFACE-001, 2026-08-20 — prod promotion; CX-004 P0 override)

PriorityFloor:
P5 — subordinated to P0 contrast/readability
```
