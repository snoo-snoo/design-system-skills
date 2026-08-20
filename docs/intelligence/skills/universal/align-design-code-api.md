# SKILL: align-design-code-api

```text
SKILL: align-design-code-api

PURPOSE:
Ensure design-tool component props/variants map cleanly to the implementation API.

SCOPE / WHEN TO USE:
- Authoring/updating design-system components
- Reviewing Figma libraries vs code packages
- Preventing unimplementable prop matrices

INPUTS:
- Design component property model
- Code component API (props/variants/slots/states)

RULES:
1. MUST map design properties to implementation API (RULE-COMPONENT-API-001).
2. SHOULD document the design↔code mapping.
3. SHOULD prefer composable props over combinatorial explosions.
4. SHOULD co-design with engineering for system components.
5. MUST NOT ship production system components with Figma-only unimplementable props.

CONSTRAINTS / DON'T:
- Don't treat marketing comps as system API.
- Don't invent token/prop names that don't exist in code.

DECISION LOGIC: (P0–P7)
P4 system consistency; never invent a11y-breaking APIs to match a mock.

ACCESSIBILITY:
API must still expose accessible names/states required by CORE a11y rules.

OUTPUT REQUIREMENTS:
- Prop mapping table (design → code)
- Gaps / rename proposals
- Explicit non-API annotations

VALIDATION / SELF-REVIEW:
- [ ] Every design prop has a code counterpart or is marked non-API
- [ ] No unimplementable boolean matrices
- [ ] Names aligned or migration noted

RELATED SKILLS: apply-spacing-scale, apply-semantic-color, apply-radius-scale
SOURCE RULES: RULE-COMPONENT-API-001
```
