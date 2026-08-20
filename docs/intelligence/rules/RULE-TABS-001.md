# RULE-TABS-001 — Tabs Structure & Keyboard

```text
RULE-TABS-001
Name: Tabs Structure & Keyboard
Category: 03 Components / Tabs + 06 Accessibility
Principle: PRINCIPLE-TABS-001
Recommendation:
  MUST structure tabs as tablist > tab with associated tabpanel.
  MUST expose exactly one aria-selected="true" tab at a time.
  MUST associate tabs and panels (aria-controls / aria-labelledby).
  MUST support arrow-key navigation within the tab list; Tab moves into the
  active panel / page sequence.
  SHOULD use automatic activation when panels are fast/preloaded; otherwise
  manual activation (Space/Enter) per APG.
  MUST set aria-orientation="vertical" when the tab list is vertical.
Reason:
  Fake tabs (plain links/buttons without tab semantics) break AT structure
  and keyboard expectations.
Context:
  In-page tabbed content (not primary site navigation unless designed as tabs).
Exceptions:
  Carousel-like patterns; segmented controls that are not tabpanels;
  progressive enhancement to native select on small screens (document alternate).
Anti-pattern:
  Visually tabbed panels implemented only as styled links with no roles/state.
  All panels in DOM visible to AT without selection state.
  Only Tab key (no arrows) to move between tabs inside the list.
Evidence:
  - ST-002 APG Tabs Pattern
  - ST-003 Heuristics #4 Consistency, #6 Recognition over recall
Confidence: High
Maturity: CORE
Related Rules: RULE-FOCUS-001, RULE-DIALOG-001
PriorityFloor: P0 (semantics/keyboard); P3 (visual selection styling)
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE from PRINCIPLE-TABS-001 (Wave-A)
```

## Attribution

| Field | Value |
| --- | --- |
| Rule ID | RULE-TABS-001 |
| Source IDs | ST-002, ST-003 |
| Normalized from | PRINCIPLE-TABS-001 |
| Synthesis | docs/intelligence/synthesis/wave-a.md |
| Confidence | High |
| Last reviewed | 2026-08-20 |

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear, reusable, contextualized | ✅ |
| Evidence mix | ✅ APG + Heuristics |
| Accessibility-compatible | ✅ |
| AI-applicable + validatable | ✅ |
| Anti-pattern present | ✅ |
| Conflicts documented | ✅ |
