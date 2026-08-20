# DS-004 — Atlassian Design System (Wave B)

**Status:** analyzed (2026-08-20)  
**Pages:** [Spacing](https://atlassian.design/foundations/spacing) · [Color](https://atlassian.design/foundations/color) · [Tokens](https://atlassian.design/foundations/tokens/design-tokens) · Button appearances (Forge UI Kit / ADS button guidance)

## Claim inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| ATL-S1 | Spacing uses a limited token scale on an 8px base (`space.*`); prefer tokens over raw px/rem | System Convention | High |
| ATL-S2 | Proximity + similarity grouping create semantic relationships; whitespace creates hierarchy | Practice + Heuristic | High |
| ATL-S3 | Optical adjustments stay on the spacing scale | System Convention | Medium–High |
| ATL-C1 | Apply color via design tokens (property + role + emphasis + state), not raw shades | System Convention | High |
| ATL-C2 | Color **roles** carry intent (neutral, brand, information, success, warning, danger, …) | System Convention | High |
| ATL-C3 | Don’t use accent when the color has semantic meaning | Practice / Constraint | High |
| ATL-C4 | Themes (light/dark) remap token values; designers shouldn’t hand-map hex for themes | System Convention | High |
| ATL-C5 | WCAG AA contrast targets called out for text / essential UI | Standard-aligned | High |
| ATL-B1 | Primary button = most important CTA; **once per area** | Practice | High |
| ATL-B2 | Default for most non-primary actions; subtle often pairs as Cancel | Practice | High |
| ATL-B3 | Danger = final confirmation of destructive/irreversible action | Practice | High |
| ATL-B4 | Warning = significant change / possible data loss confirms | Practice | Medium–High |
| ATL-B5 | Prefer validation over disabled primary submit when possible (disabled buttons hurt a11y discoverability) | Practice + A11y | Medium–High |

## Principle links

- Hardens RULE-SPACE-001 / RULE-COLOR-001  
- Promotes COLOR-RESTRAINT (semantic over decorative accent)  
- Seeds PRINCIPLE-ACTION-HIERARCHY-001 → CORE  
- Feeds FORM-FEEDBACK / disabled-button caveat (CANDIDATE note)

## Notes

- Token numeric suffixes (space.100 etc.) are Atlassian-specific — extract the **principle**, not the numbers.  
- ATL-B5 recorded; do not elevate to CORE “never disable” without broader synthesis (CX watch).
