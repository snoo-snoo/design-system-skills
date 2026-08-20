# SKILL: size-touch-targets

```text
SKILL: size-touch-targets

PURPOSE:
Ensure interactive pointer targets meet accessibility minimums and remain
comfortable for primary mobile actions.

SCOPE / WHEN TO USE:
- Designing or reviewing buttons, icons, chips, list rows, form controls
- Mobile / touch-first flows (auth, checkout, payments)
- Dense toolbars where hit areas shrink

INPUTS:
- Control inventory with sizes and spacing
- Platform (mobile/desktop) and primary vs secondary actions
- Design-system control size tokens if available

RULES:
1. MUST meet WCAG 2.2 Target Size (Minimum) for applicable controls (RULE-TOUCH-001).
2. SHOULD use comfortable thumb-friendly targets for primary mobile actions.
3. MAY enlarge hit area with padding without enlarging the visual.
4. SHOULD use system size tokens (e.g. Primer control sizes) when available.
5. MUST NOT pack undersized adjacent targets that cause mis-taps.

CONSTRAINTS / DON'T:
- Don't shrink icon buttons below minimum without an expanded hit box.
- Don't invent token values — snap to the project scale.
- Don't treat inline-link WCAG exceptions as license for tiny primary CTAs.

DECISION LOGIC: (P0–P7)
P0 minimum size is mandatory. Comfort sizing is SHOULD. Density aesthetics (P5–P7)
cannot override minimums.

ACCESSIBILITY:
WCAG 2.5.8. Pair with ensure-visible-focus for keyboard users.

OUTPUT REQUIREMENTS:
- Per-control target size (visual + hit area)
- Token mapping if DS present
- Failures and proposed fixes

EDGE CASES:
- Inline text links (exception paths)
- Nested hit targets inside list rows
- Hover-only enlarge patterns (not a substitute for base size)

VALIDATION / SELF-REVIEW:
- [ ] Applicable controls meet minimum target size
- [ ] Primary mobile actions are comfortably tappable
- [ ] Adjacent controls have adequate separation or hit areas
- [ ] No magic undersized icon buttons

RELATED SKILLS: ensure-visible-focus, label-form-fields
SOURCE RULES: RULE-TOUCH-001
```
