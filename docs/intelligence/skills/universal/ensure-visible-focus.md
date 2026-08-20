# SKILL: ensure-visible-focus

```text
SKILL: ensure-visible-focus

PURPOSE:
Ensure every interactive control has a visible, unobscured keyboard focus
indicator and a coherent focus order.

SCOPE / WHEN TO USE:
- Generating or reviewing UI with buttons, links, inputs, menus, dialogs
- Fixing “focus ring removed” or sticky-header occlusion bugs
- Prefacing modal work (also use build-accessible-modal)

INPUTS:
- UI description, component tree, or code/CSS for interactive elements
- Known overlays / sticky regions
- Design-system focus tokens if available

RULES:
1. MUST provide a visible focus style for every focusable control (RULE-FOCUS-001).
2. MUST NOT remove outline/ring without an equivalent or stronger replacement.
3. MUST keep focused elements from being fully covered by sticky/overlay chrome.
4. MUST preserve a logical focus order matching the reading/interaction model.
5. SHOULD use system focus tokens when a design system is in play.

CONSTRAINTS / DON'T:
- Don't hide focus for “clean aesthetics” (P7 loses to P0).
- Don't make non-interactive chrome focusable.
- Don't invent contrast-failing focus colors when tokens exist.

DECISION LOGIC: (P0–P7)
P0 Accessibility wins over brand minimalism. If brand style conflicts with
visibility, keep brand color but ensure contrast and occlusion safety.

ACCESSIBILITY:
Maps to WCAG 2.4.7 and 2.4.11. Coordinate with modal focus trap skills.

OUTPUT REQUIREMENTS:
- List of focusable elements checked
- Focus treatment specified (token or concrete style)
- Notes on sticky/overlay occlusion risks
- Pass/fail self-review checklist

EDGE CASES:
- Disabled controls (usually not focusable)
- Nested scroll regions
- Focus inside open dialogs (defer trap details to build-accessible-modal)

VALIDATION / SELF-REVIEW:
- [ ] No focusable control lacks a visible focus state
- [ ] No outline:none / ring-0 without replacement
- [ ] Sticky headers/footers do not fully hide focused targets
- [ ] Tab order matches structure

RELATED SKILLS: build-accessible-modal, size-touch-targets
SOURCE RULES: RULE-FOCUS-001
```
