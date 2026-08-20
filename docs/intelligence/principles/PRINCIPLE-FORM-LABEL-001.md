# PRINCIPLE-FORM-LABEL-001 — Persistent Visible Field Labels

```text
Principle:
Form fields should keep a persistent, visible label (typically above the
control); do not rely on placeholder-only or disappearing labels.

Problem:
Missing/disappearing labels cause errors, skipped fields, zoom issues, and
AT confusion.

Recommendation:
Always show a short descriptive label. Use placeholder/hint for format help
only. Prefer persistent labels over floating-label-as-default.

Why:
Clarity, accessibility, localization, and error recovery.

Context:
All data-entry forms (settings, onboarding, checkout, fintech).

Exceptions:
Severely constrained search fields with visible nearby legend; highly tested
specialized patterns that still expose accessible names persistently to AT.
Floating labels may appear in brand products but remain non-default here.

Evidence:
- ST-001 WCAG labels/instructions (3.3.2) directionally
- Community a11y critique on VID-SAMPLE-004 floating labels (LinkedIn)
- Creator’s related teaching against placeholder-as-label (cross-post corpus)

Confidence:
High

Category:
04 Patterns / Forms + 07 Content + 06 Accessibility

StatementClass:
Practice elevated by Standard pressure + expert consensus against contested pattern

Maturity:
CORE (formalized as RULE-FORM-LABEL-001, 2026-08-20; CX-003 default)

PriorityFloor:
P0
```
