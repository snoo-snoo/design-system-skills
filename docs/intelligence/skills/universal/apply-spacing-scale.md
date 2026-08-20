# SKILL: apply-spacing-scale

```text
SKILL: apply-spacing-scale

PURPOSE:
Lay out UI using the project’s discrete spacing token scale—never arbitrary
magic-number margins/paddings.

SCOPE / WHEN TO USE:
- Generating layouts, stacks, component padding
- Refactoring inconsistent spacing
- Reviewing AI-generated UI for off-scale values

INPUTS:
- Project spacing tokens / scale (required if available)
- Layout structure (stacks, grids, sections)
- Breakpoints

RULES:
1. MUST use spacing tokens from the project scale (RULE-SPACE-001).
2. MUST NOT invent new px/rem spacing values when tokens exist.
3. SHOULD prefer parent gap/stack spacing over per-child unique margins.
4. SHOULD change spacing at breakpoints by jumping token steps.
5. MUST document rare optical exceptions explicitly.

CONSTRAINTS / DON'T:
- Don't hard-code 13px / 27px “eyeball” spacing.
- Don't invent a new global scale if the product already has one.
- Don't sacrifice touch targets (RULE-TOUCH-001) to tighten spacing.

DECISION LOGIC: (P0–P7)
P4 system consistency governs spacing choices. If spacing conflicts with
P0 target size or focus visibility, enlarge hit area/focus first.

ACCESSIBILITY:
Spacing supports hierarchy and target separation; never reduce below
accessible target needs.

OUTPUT REQUIREMENTS:
- Tokenized spacing map for the layout
- List of any off-scale exceptions with rationale
- Confirmation that no magic numbers were introduced

EDGE CASES:
- Percentage-based page splits
- Third-party embeds
- Optical alignment of icons/text (±1px) — document if unavoidable

VALIDATION / SELF-REVIEW:
- [ ] All spacing maps to tokens (or documented exception)
- [ ] Stacks/gaps preferred over scattered margins
- [ ] Responsive steps use scale jumps
- [ ] Touch targets still meet RULE-TOUCH-001

RELATED SKILLS: apply-semantic-color, size-touch-targets
SOURCE RULES: RULE-SPACE-001
```
