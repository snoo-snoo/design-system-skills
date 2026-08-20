# Analysis — DS-002 Carbon Foundations (Spacing + Color)

**Sources:**  
- https://carbondesignsystem.com/elements/spacing/overview/  
- https://carbondesignsystem.com/elements/color/overview/  
**Captured:** 2026-08-20 · **Status:** analyzed (Foundations slice)

## Claims inventory

| ID | Claim | Class | Confidence |
| --- | --- | --- | --- |
| CB-S1 | Use a discrete spacing scale (2/4/8 multiples) via tokens for margin/padding | System Convention | High |
| CB-S2 | Nearness implies relationship; more space weakens perceived relationship | Heuristic (Gestalt-aligned) | High |
| CB-S3 | More surrounding space → higher perceived importance | Heuristic | Medium |
| CB-S4 | White space prevents overload; whole page should not be dense | Heuristic / Practice | Medium |
| CB-S5 | Deviate from spacing scale only as rare exception | System Convention | Medium |
| CB-S6 | Spacing tokens are not themselves responsive; jump scale steps at breakpoints | System Convention | High |
| CB-S7 | Prefer Stack/layout parents over component-owned margins | System Practice | Medium |
| CB-C1 | Color via role-based tokens + themes (not raw hex in product UI) | System Convention | High |
| CB-C2 | Layering model stacks neutrals differently in light vs dark themes | System Convention | High |
| CB-C3 | Interaction states (hover/active/selected/focus/disabled) have explicit token logic | System Convention | High |
| CB-C4 | Focus typically 2px border; must meet ~3:1; often needs focus-inset | System Convention + A11y | High |
| CB-C5 | Disabled styling intentionally de-emphasized; not subject to WCAG contrast like enabled UI | System Convention | High (as Carbon policy) |
| CB-C6 | Small text contrast 4.5:1 / large 3:1 / graphics 3:1 per WCAG framing | Standard (via Carbon) | High |

## Radius note

No authoritative nested-radius formula found on Carbon spacing/color pages in this capture. Corner-radius guideline URL redirected/404 during capture. **Does not contradict** PRINCIPLE-RADIUS-001; also does not confirm it.

## Principle candidates spawned

- PRINCIPLE-SPACE-001 (tokenized spacing scale)
- PRINCIPLE-COLOR-001 (semantic color tokens + themes)
- PRINCIPLE-FOCUS-001 (explicit focus treatment) — also from APG/WCAG

## Next

Typography + 2x Grid pages; component a11y crosswalk for Button/Modal.
