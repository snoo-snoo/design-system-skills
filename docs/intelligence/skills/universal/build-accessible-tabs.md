# SKILL: build-accessible-tabs

```text
SKILL: build-accessible-tabs

PURPOSE:
Build or audit in-page tabs with correct roles, selection state, and
arrow-key keyboard interaction.

SCOPE / WHEN TO USE:
- Tabbed settings, detail panels, in-page section switching
- Replacing “fake tabs” built from plain links/buttons
- Not for primary site navigation unless intentionally designed as tabs

INPUTS:
- Tab labels + panel content
- Orientation (horizontal/vertical)
- Activation mode preference (automatic vs manual)
- Framework constraints

RULES:
1. MUST use tablist > tab + associated tabpanel (RULE-TABS-001).
2. MUST keep exactly one aria-selected="true" tab.
3. MUST wire aria-controls / aria-labelledby associations.
4. MUST support arrow keys in the tab list; Tab moves into the active panel.
5. SHOULD prefer automatic activation when panels are fast; else manual
   (Space/Enter) per APG.
6. MUST set aria-orientation="vertical" when vertical.

CONSTRAINTS / DON'T:
- Don't style links as tabs without roles/state.
- Don't expose all panels to AT as equally active.
- Don't rely only on Tab to move between tabs inside the list.

DECISION LOGIC: (P0–P7)
P0 semantics/keyboard first; visual selection styling is P3.

ACCESSIBILITY:
APG Tabs Pattern. Pair with ensure-visible-focus for tab/panel focus styles.

OUTPUT REQUIREMENTS:
- Role tree
- Keyboard map
- Selection/activation behavior
- Orientation attribute if needed

EDGE CASES:
- Segmented controls that are not tabpanels
- Progressive enhancement to select on small screens
- Lazy-loaded panels (favor manual activation)

VALIDATION / SELF-REVIEW:
- [ ] Correct roles and single selection
- [ ] Panels labelled by their tabs
- [ ] Arrow-key navigation works
- [ ] Tab key enters the active panel

RELATED SKILLS: ensure-visible-focus, build-accessible-modal
SOURCE RULES: RULE-TABS-001, RULE-FOCUS-001
```
