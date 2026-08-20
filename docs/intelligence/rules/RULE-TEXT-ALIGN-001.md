# RULE-TEXT-ALIGN-001 — Prefer Start Alignment for Multi-line UI Text

```text
RULE-TEXT-ALIGN-001
Name: Prefer Start Alignment for Multi-line UI Text
Category: 02 Layout / Alignment + 01 Typography
Principle: PRINCIPLE-TEXT-ALIGN-001
Recommendation:
  SHOULD use start alignment (left in LTR; logical start in RTL) for body copy,
  lists, form copy, and multi-line descriptions in product UI.
  MUST NOT stack multiple lines of center-aligned text as the default for
  readable content blocks.
  MAY center short headlines, single-line labels, or intentional hero/empty-state
  titles.
Reason:
  Centered multi-line text weakens alignment anchors and slows scanning.
Context:
  Product UI layouts (web/mobile). Marketing compositions may differ.
Exceptions:
  Short centered headings; poetry/quotes; single-line CTAs; decorative marketing.
Anti-pattern:
  Long centered paragraphs in settings/forms/dashboards.
  Mixing start and center randomly within one content column.
Evidence:
  - VID-SAMPLE-005
  - Typography craft / scanability practice
  - Aligns with hierarchy goals (P2) and RULE-SPACE-001 rhythm
Confidence: Medium–High
Maturity: CORE
Related Rules: RULE-SPACE-001, RULE-FORM-LABEL-001
PriorityFloor: P2 information hierarchy / P5 craft
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE by product decision (CANDIDATE → prod)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Exceptions | ✅ |
| AI-validatable | ✅ |
| Anti-pattern | ✅ |
