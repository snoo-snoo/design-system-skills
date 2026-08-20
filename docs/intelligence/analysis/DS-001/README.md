# DS-001 — Material Design 3 Foundations (Wave B)

**Status:** analyzed (2026-08-20)  
**Pages:** Design tokens overview · Shape scale (via M3 / material-web / Compose docs) · Layout spacing principles (grids & spacing IA)  
**Capture note:** m3.material.io pages are JS-heavy; claims corroborated via Material Web shape tokens + Android/Compose M3 shape docs.

## Claim inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| M3-T1 | Design tokens are the shared building blocks across design and code | System Convention | High |
| M3-S1 | Layout/spacing uses a consistent spacing scale (commonly 4dp increments in Material layout guidance) | System Convention | Medium–High |
| M3-R1 | Shape uses a **corner radius scale** (none → extra-small → small → medium → large → extra-large → full) | System Convention | High |
| M3-R2 | Components map to shape roles rather than one-off radii | System Convention | High |
| M3-C1 | Color is applied via roles in schemes/themes (not raw one-off hex in product UI) | System Convention | High |

## Principle links

- Reinforces PRINCIPLE-SPACE-001 / RULE-SPACE-001  
- Promotes PRINCIPLE-RADIUS-SCALE-001 → CORE  
- Reinforces PRINCIPLE-COLOR-001 / RULE-COLOR-001  

## Notes

- Do not copy Material visual language wholesale; extract scale/token structure.  
- Exact dp values are system-specific — never invent values for other products.
