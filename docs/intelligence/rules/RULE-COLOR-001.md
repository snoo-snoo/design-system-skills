# RULE-COLOR-001 — Semantic Color Tokens + Themes

```text
RULE-COLOR-001
Name: Semantic Color Tokens + Themes
Category: 01 Foundations / Color
Principle: PRINCIPLE-COLOR-001
Recommendation:
  MUST apply product UI color through role-based semantic tokens (and themes),
  not raw palette hex/rgb in surfaces/components.
  MUST map roles (background, layer, text, border, support/status, focus, etc.)
  by theme (light/dark/high-contrast as applicable).
  SHOULD implement interaction states via dedicated state tokens.
  SHOULD reserve high-salience color for action, status, and intentional emphasis.
  MUST meet contrast requirements for text and required non-text UI (P0).
Reason:
  Hard-coded colors break theming, drift state language, and undermine
  contrast governance.
Context:
  Multi-theme product UIs and design-system-backed applications.
Exceptions:
  Data visualization scales.
  Marketing/brand moments outside the product shell.
  Documented inverse/high-contrast components.
  Illustrations / photography.
Anti-pattern:
  Hex sprinkled in component styles for text/background/border.
  Using brand accent for large body text areas without semantic role.
  Inventing off-theme colors for “this one screen.”
Evidence:
  - DS-002 Carbon Color overview (tokens, themes, layering, states, a11y)
  - Cross-aligns with DS study matrix token APIs (Polaris/Atlassian)
  - Wave-A synthesis consensus
Confidence: High
Maturity: CORE
Related Rules: RULE-FOCUS-001, RULE-SPACE-001
PriorityFloor: P0 for contrast-related roles; P4 for token discipline
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-COLOR-001 (Wave-A)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-COLOR-001 |
| Source IDs | DS-002 (+ DS matrix) |
| Normalized from | PRINCIPLE-COLOR-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ Flagship DS + matrix alignment |
| Accessibility-compatible | ✅ contrast = P0 |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ viz/brand exceptions; CX-002 not elevated |
