# PRINCIPLE-COLOR-001 — Semantic Color Tokens + Themes

```text
Principle:
Apply color through role-based tokens and themes, not raw palette values
in product surfaces.

Problem:
Hard-coded hex causes theme breakage, inconsistent states, and a11y drift.

Recommendation:
Use semantic roles (background, layer, text, border, support/status, focus,
etc.) mapped by theme. Implement interaction states via dedicated state
tokens. Reserve high-salience color for action/status/emphasis.

Why:
Scalable theming (light/dark/high-contrast), consistent state language,
easier contrast governance.

Context:
Multi-theme product UIs and design-system-backed apps.

Exceptions:
Data visualization scales; marketing/brand moments; documented high-contrast
inverse components; illustrations.

Evidence:
- DS-002 Carbon Color overview (tokens, themes, layering, states, a11y)
- Cross-aligns with general DS study matrix (Polaris/Atlassian token APIs)

Confidence:
High

Category:
01 Foundations / Color

StatementClass:
System Convention

Maturity:
CORE (formalized as RULE-COLOR-001, 2026-08-20; Carbon + DS matrix)

PriorityFloor:
P0 for contrast-related roles; P4 for general token discipline
```
