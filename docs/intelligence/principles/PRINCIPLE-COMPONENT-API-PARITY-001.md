# PRINCIPLE-COMPONENT-API-PARITY-001 — Design Props Match Implementation API

```text
Principle:
Component properties defined in design tools must map cleanly to the
implementation component API (props/variants/slots); design and code share
one contract.

Problem:
Figma-only prop models that ignore code constraints cause drift, one-off
hacks, and design-system breakage between design and engineering.

Recommendation:
When authoring components, define variants/props with the implementation API
in mind (boolean vs enum, slots vs nested instances, state vs variant).
Document the mapping. Prefer fewer, composable props over unimplementable
combinatorial matrices. Pair designers and engineers on API design.

Why:
A design system is a product contract across tools; parity keeps tokens,
components, and docs trustworthy.

Context:
Design-system libraries, shared UI kits, multi-platform component sets.
React is a common case but the rule is framework-agnostic.

Exceptions:
Exploratory throwaway prototypes; marketing comps not destined for the system;
intentional design-only annotations clearly marked non-API.

Evidence:
- VID-SAMPLE-007
- Broader DS practice: systems-as-engineering-product (Primer/Carbon governance signals)
- Related: token contracts already treated as APIs in this repo’s DS analyses

Confidence:
Medium–High

Category:
03 Components + Design System Architecture

StatementClass:
Practice / Workflow

Maturity:
CANDIDATE

PriorityFloor:
P4 design-system consistency
```
