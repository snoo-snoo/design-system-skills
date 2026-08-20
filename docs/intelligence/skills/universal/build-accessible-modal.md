# SKILL: build-accessible-modal

```text
SKILL: build-accessible-modal

PURPOSE:
Specify or implement a modal dialog that is named, focus-trapped,
Esc-dismissible, and restores focus on close.

SCOPE / WHEN TO USE:
- Adding confirmations, forms-in-overlay, multi-step modal flows
- Auditing custom overlay/modal components
- Not for non-modal popovers/dropdowns (different pattern)

INPUTS:
- Dialog purpose + title text
- Trigger element
- Content risk (destructive vs informational)
- Framework / native <dialog> availability

RULES:
1. MUST name the dialog (aria-labelledby preferred) (RULE-DIALOG-001).
2. MUST make true modals modal for everyone (background not operable).
3. MUST move focus into the dialog on open.
4. MUST trap Tab / Shift+Tab inside while open.
5. MUST support Escape + a visible close/cancel control in tab order.
6. MUST restore focus to the invoker on close (unless documented exception).
7. SHOULD choose initial focus based on risk (e.g. avoid focusing destructive
   confirm by default when a safer control exists).

CONSTRAINTS / DON'T:
- Don't use a plain div overlay without dialog semantics.
- Don't leave focus on the trigger while the modal is open.
- Don't allow background tab stops.
- Don't confuse non-modal dialogs with this skill’s MUST list.

DECISION LOGIC: (P0–P7)
P0 operable modal behavior overrides visual “sheet” aesthetics.

ACCESSIBILITY:
APG Dialog (Modal) Pattern; coordinate with ensure-visible-focus.

OUTPUT REQUIREMENTS:
- Role/name wiring
- Open/close focus plan
- Keyboard behavior notes
- Close control placement

EDGE CASES:
- alertdialog
- Nested dialogs (avoid when possible; if required, document stack rules)
- Native <dialog> with equivalent behaviors

VALIDATION / SELF-REVIEW:
- [ ] Accessible name present
- [ ] Focus moves in on open and restores on close
- [ ] Tab cycles inside; Esc dismisses
- [ ] Background inert while open
- [ ] Visible dismiss control in tab order

RELATED SKILLS: ensure-visible-focus, build-accessible-tabs
SOURCE RULES: RULE-DIALOG-001, RULE-FOCUS-001
```
