# RULE-COLOR-RESTRAINT-001 — Restrained Non-Semantic Color

```text
RULE-COLOR-RESTRAINT-001
Name: Restrained Non-Semantic Color
Category: 01 Foundations / Color
Principle: PRINCIPLE-COLOR-RESTRAINT-001
Recommendation:
  MUST apply meaningful color through semantic roles (action, status, emphasis,
  brand-intent) via tokens (see RULE-COLOR-001).
  SHOULD default most surfaces/text/icons to neutrals.
  MUST NOT use decorative accent colors where a semantic role is required
  (e.g. don’t use interchangeable accent for danger/success meaning).
  SHOULD add strong color only when it communicates meaning or a deliberate
  brand moment.
Reason:
  Excess unrelated color increases noise and weakens hierarchy/consistency.
Context:
  Product UI (SaaS, admin, consumer apps). Marketing surfaces may differ.
Exceptions:
  Data visualization categorical scales; brand-heavy campaigns; high-contrast
  modes (still semantic).
Anti-pattern:
  Rainbow icon rows with no meaning.
  Using a random accent for error/destructive states.
Evidence:
  - DS-002 Carbon Color (“additional colors used sparingly”)
  - DS-004 Atlassian Color (“Don’t use an accent when the color has semantic meaning”)
  - VID-SAMPLE-002 (supporting Practice)
  - RULE-COLOR-001
Confidence: High
Maturity: CORE
Related Rules: RULE-COLOR-001, RULE-ACTION-001
PriorityFloor: P4 system / P5 craft; never override contrast (P0)
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE in Wave B (Atlassian accent rule + Carbon)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Evidence mix | ✅ |
| A11y compatible | ✅ |
| Anti-pattern | ✅ |
