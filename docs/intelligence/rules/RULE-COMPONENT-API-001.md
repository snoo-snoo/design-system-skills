# RULE-COMPONENT-API-001 — Design Props Match Implementation API

```text
RULE-COMPONENT-API-001
Name: Design Props Match Implementation API
Category: 03 Components + Design System Architecture
Principle: PRINCIPLE-COMPONENT-API-PARITY-001
Recommendation:
  MUST define design-tool component properties so they map cleanly to the
  implementation API (props/variants/slots/states).
  SHOULD document the design↔code mapping for shared components.
  SHOULD prefer fewer, composable props over unimplementable combinatorial matrices.
  SHOULD co-design APIs with engineering when adding system components.
  MUST NOT invent Figma-only props that cannot be implemented without hacks
  for production system components.
Reason:
  Drift between design and code breaks the design-system contract.
Context:
  Design-system libraries, shared UI kits, multi-platform component sets.
Exceptions:
  Throwaway prototypes; marketing comps not destined for the system;
  design-only annotations clearly marked non-API.
Anti-pattern:
  Boolean explosion in Figma that code cannot express.
  Divergent variant names between design library and package API.
Evidence:
  - VID-SAMPLE-007
  - DS governance practice (systems as engineering products; token APIs in DS analyses)
  - Aligns with RULE-SPACE-001 / RULE-COLOR-001 token contracts
Confidence: Medium–High
Maturity: CORE
Related Rules: RULE-SPACE-001, RULE-COLOR-001, RULE-RADIUS-SCALE-001
PriorityFloor: P4 design-system consistency
LastReviewed: 2026-08-20
Changelog:
  - 2026-08-20: Promoted CORE by product decision (CANDIDATE → prod)
```

## Quality Gate

| Check | Pass |
| --- | --- |
| Clear + reusable | ✅ |
| AI-applicable | ✅ |
| Anti-pattern | ✅ |
