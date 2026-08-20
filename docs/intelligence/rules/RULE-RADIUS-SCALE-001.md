# RULE-RADIUS-SCALE-001 — Semantic Radius / Shape Scale

```text
RULE-RADIUS-SCALE-001
Name: Semantic Radius / Shape Scale
Category: 01 Foundations / Radius
Principle: PRINCIPLE-RADIUS-SCALE-001
Recommendation:
  MUST pick border radii from the project’s limited semantic radius/shape scale
  (e.g. none/sm/md/lg/full or equivalent roles), not arbitrary one-off px values.
  SHOULD map components to radius roles consistently (cards, controls, overlays).
  SHOULD reserve full/pill radii for truly pill-shaped controls.
  MAY combine with nested-radius craft (PRINCIPLE-RADIUS-001) when composing
  nested surfaces — still snap results to the scale when a scale exists.
  MUST NOT invent new radius tokens when generating UI.
Reason:
  Arbitrary radii fragment visual language and break theming/lintability.
Context:
  Design-system-backed product UIs.
Exceptions:
  Marketing illustration; intentional brand moments; platform-native controls.
Anti-pattern:
  Every card/modal gets a unique radius (11px, 13px, 18px…).
  Pill radius on large rectangular content containers.
Evidence:
  - DS-005 Primer borderRadius tokens
  - DS-003 Polaris shape tokens / Card defaults
  - DS-001 Material 3 shape scale (none → extra-small → … → full)
Confidence: High
Maturity: CORE
Related Rules: RULE-SPACE-001, RULE-COLOR-001
PriorityFloor: P4
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE in Wave B (Material shape scale + Primer/Polaris)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Evidence mix (≥2 systems + Material) | ✅ |
| A11y compatible | ✅ |
| AI-validatable | ✅ |
| Anti-pattern | ✅ |
