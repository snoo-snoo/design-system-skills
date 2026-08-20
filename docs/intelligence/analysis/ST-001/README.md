# Analysis Report — ST-001 (WCAG 2.2)

**Source:** [ST-001](../../sources/ST-001.md)  
**Captured:** 2026-08-20  
**Status:** `in_analysis` (Wave A kickoff map)

## 1. Source Summary

W3C Recommendation (2024-12-12). Normative, testable success criteria under POUR. Supporting Understanding/Techniques docs are informative.

## 2. Key Insights for Design System Intelligence

- Accessibility rules from WCAG are **P0** and can become CORE when mapped to UI patterns.
- Prefer **AA** as default product bar unless product policy says otherwise; document level on every rule.
- WCAG does **not** prescribe corner radius, color palettes for brand, or aesthetic minimalism.

## 3. Taxonomy map (AA focus — starter)

| Area | Example SC (non-exhaustive) | Taxonomy |
| --- | --- | --- |
| Contrast | 1.4.3 Contrast (Minimum), 1.4.11 Non-text Contrast | 01 Color / 06 A11y |
| Resize / Reflow | 1.4.4, 1.4.10 | 08 Responsive |
| Keyboard | 2.1.1, 2.1.2 | 06 A11y / 03 Components |
| Focus visible | 2.4.7 | 06 A11y |
| Focus not obscured | 2.4.11 (2.2) | 06 A11y / Overlays |
| Target size | 2.5.8 (2.2) | 01 Sizing / 06 A11y |
| Dragging alternatives | 2.5.7 (2.2) | 05 Interaction |
| Labels / Instructions | 3.3.2 | 07 Content / Forms |
| Error identification | 3.3.1, 3.3.3 | 04 Error States |
| Accessible auth | 3.3.7, 3.3.8 (2.2) | 04 Authentication |
| Status messages | 4.1.3 | 04 Feedback / 09 AI UI status |

## 4. Claim inventory (meta)

| Claim | Class | Confidence |
| --- | --- | --- |
| Success criteria are normative requirements for conformance | Standard | High |
| Techniques are one way, not the only way | Standard (informative layer) | High |
| AAA is not a universal default product mandate | Practice / Policy | Medium |

## 5. Potential CORE rule seeds (Phase 5 later)

- Focus visibility & non-obscured focus for overlays/sticky chrome
- Minimum target size for pointer inputs
- Non-text contrast for UI components and states
- Error identification + suggestion in forms

## 6. Conflicts / non-goals

- Does not validate aesthetic tips (e.g. nested radius formula from VID-SAMPLE-001)
- Cognitive guidance remains incomplete per WCAG intro — don’t overclaim

## 7. Next analysis steps

1. Deep-dive pages for 2.4.11, 2.5.8, 1.4.11 → principle cards  
2. Crosswalk to APG (ST-002) for dialogs/tabs  
3. Crosswalk to Carbon/Polaris component a11y sections
