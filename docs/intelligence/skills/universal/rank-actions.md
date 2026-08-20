# SKILL: rank-actions

```text
SKILL: rank-actions

PURPOSE:
Establish a clear action hierarchy: one primary per area, restrained danger, clear secondaries.

SCOPE / WHEN TO USE:
- Toolbars, forms, dialogs, headers, empty states
- Resolving competing CTA designs

INPUTS:
- Action list with outcomes (primary goal, secondary, destructive)
- Region/view boundaries

RULES:
1. MUST establish a clear visual hierarchy of actions (RULE-ACTION-001).
2. SHOULD use one primary CTA per area for the most important action.
3. SHOULD style ordinary actions as default/secondary; Cancel as subtle/link when paired.
4. MUST reserve danger for final destructive irreversible confirms.
5. SHOULD use warning (if available) for significant change / data-loss confirms.
6. SHOULD prefer validation feedback over unexplained disabled primaries (CX-006).

CONSTRAINTS / DON'T:
- Don't place multiple primaries in the same region.
- Don't use danger styling for emphasis on safe actions.

DECISION LOGIC: (P0–P7)
Preventing irreversible harm (danger misuse) is P0-adjacent; clarity is P1; consistency P3.

ACCESSIBILITY:
Keep targets sized (RULE-TOUCH-001) and focus visible; loading buttons must not lose accessible names.

OUTPUT REQUIREMENTS:
- Action → style role map (primary/default/subtle/warning/danger)
- Region primary identified
- Destructive confirm plan

EDGE CASES:
- Multi-region dashboards; icon-only actions; split buttons

VALIDATION / SELF-REVIEW:
- [ ] ≤1 primary per area
- [ ] Danger only on destructive confirms
- [ ] Cancel/secondary ranking clear
- [ ] No unexplained disabled primary

RELATED SKILLS: provide-form-feedback, build-accessible-modal, restrain-decorative-color
SOURCE RULES: RULE-ACTION-001
```
