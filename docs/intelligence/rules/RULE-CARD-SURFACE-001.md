# RULE-CARD-SURFACE-001 — Card Chrome Only When Needed

```text
RULE-CARD-SURFACE-001
Name: Card Chrome Only When Needed
Category: 03 Components / Cards
Principle: PRINCIPLE-CARD-SURFACE-001
Recommendation:
  SHOULD NOT wrap every content block in a filled/bordered card by default.
  SHOULD prefer spacing, typography, and selective dividers for hierarchy first.
  MAY use filled/bordered cards when containment, interactivity affordance, or
  contrast against a busy background is needed.
  MUST keep adequate contrast and target separation (P0) — never remove card
  chrome if doing so harms readability or accessibility (CX-004).
Reason:
  Ubiquitous card fills create noise; missing needed surfaces harm readability.
Context:
  Feeds, lists, dashboards, media-forward product UIs.
Exceptions:
  Dense enterprise lists needing separation; low-contrast media; accessible
  touch grouping; forms in elevated surfaces.
Anti-pattern:
  Card-wrapping every paragraph/section on a simple settings page.
  Removing all surfaces on image-heavy UIs until text fails contrast.
Evidence:
  - VID-SAMPLE-003
  - RULE-SPACE-001 / RULE-BORDER-RESTRAINT-001
  - CX-004: P0 contrast/readability overrides aesthetics
Confidence: Medium
Maturity: CORE
Related Rules: RULE-SPACE-001, RULE-BORDER-RESTRAINT-001, RULE-COLOR-001
PriorityFloor: P5 — subordinated to P0 contrast/readability
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted EXPERIMENTAL → CORE for prod completeness; CX-004
    remains as hard P0 override, not fake consensus
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| Conflicts explicit (CX-004) | ✅ |
| P0 override documented | ✅ |
| Anti-pattern | ✅ |

**Note:** Promoted for production skill coverage with mandatory P0 caveats; not a claim that borderless cards are always better.
