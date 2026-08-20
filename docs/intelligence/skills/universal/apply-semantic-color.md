# SKILL: apply-semantic-color

```text
SKILL: apply-semantic-color

PURPOSE:
Apply color through semantic role tokens and themes—not raw palette values—
while preserving contrast.

SCOPE / WHEN TO USE:
- Theming product UI (light/dark/high-contrast)
- Styling text, surfaces, borders, status, focus, actions
- Stopping hex sprawl in generated components

INPUTS:
- Design-system color roles / themes
- Component states (default, hover, active, disabled, error, success)
- Contrast requirements for text and critical non-text UI

RULES:
1. MUST use semantic color tokens for product surfaces/components (RULE-COLOR-001).
2. MUST NOT hard-code hex/rgb for text/background/border when tokens exist.
3. MUST meet contrast for text and required non-text UI (P0).
4. SHOULD map interaction states to dedicated state tokens.
5. SHOULD reserve high-salience color for action/status/emphasis.
6. MUST NOT elevate contested disabled-contrast policies without CX-002 resolution.

CONSTRAINTS / DON'T:
- Don't invent off-theme accent colors for one-off screens.
- Don't use decorative color that breaks hierarchy without a role.
- Don't treat marketing landing palettes as the product token set.

DECISION LOGIC: (P0–P7)
Contrast and focus colors are P0. Token discipline is P4. Brand expression
(P6) and aesthetic preference (P7) must not break roles or contrast.

ACCESSIBILITY:
WCAG contrast for text/non-text; focus indicators must remain visible
(RULE-FOCUS-001).

OUTPUT REQUIREMENTS:
- Role → token mapping for the UI
- State token usage
- Contrast check notes
- Exceptions (viz, brand moments) listed

EDGE CASES:
- Data visualization palettes
- Inverse/header components
- Illustrations / photos

VALIDATION / SELF-REVIEW:
- [ ] No raw hex on product text/surfaces/borders (tokens used)
- [ ] Themes switch via roles
- [ ] Contrast requirements addressed
- [ ] Focus/status colors remain semantic

RELATED SKILLS: apply-spacing-scale, ensure-visible-focus
SOURCE RULES: RULE-COLOR-001, RULE-FOCUS-001
```
