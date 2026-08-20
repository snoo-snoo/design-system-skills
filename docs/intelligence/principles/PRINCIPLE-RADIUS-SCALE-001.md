# PRINCIPLE-RADIUS-SCALE-001 — Semantic Radius Tokens

```text
Principle:
Use a limited set of semantic border-radius tokens instead of one-off px values.

Problem:
Arbitrary radii fragment visual language and break theme consistency.

Recommendation:
Pick from system radius roles (e.g. small/medium/large/full or numbered shape
tokens). Prefer full/pill only for truly pill controls. When nesting surfaces,
combine with PRINCIPLE-RADIUS-001 so chosen tokens remain concentric.

Why:
Coherent surfaces across components; lintable; themeable.

Context:
Design-system-backed product UIs.

Exceptions:
Marketing illustration; intentional brand moments; platform-native controls.

Evidence:
- DS-005 Primer borderRadius tokens
- DS-003 Polaris shape-token lint rules + Card defaults

Confidence:
High

Category:
01 Foundations / Radius

StatementClass:
System Convention

Maturity:
CANDIDATE

PriorityFloor:
P4
```
