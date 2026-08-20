# Analysis Report — ST-002 (WAI-ARIA APG)

**Source:** [ST-002](../../sources/ST-002.md)  
**Captured:** 2026-08-20  
**Status:** `in_analysis`

## 1. Source Summary

Authoring practices for ARIA design patterns: keyboard models, roles/states, landmarks, accessible names. Pattern examples are authoritative practice for web widgets.

## 2. Key Insights

- Prefer **native HTML** semantics; ARIA fills gaps.
- Component skills later must encode: roles, states, keyboard, focus movement, naming.
- Multiple implementation variants may be valid — record as options, not one true code path.

## 3. Priority patterns for Wave A/B

| Pattern | Why first | Maps to |
| --- | --- | --- |
| Dialog (Modal) | Focus trap, escape, restore focus | 03 Modals / 06 A11y |
| Tabs | Orientation, arrow keys, selection | 03 Tabs |
| Disclosure / Accordion | Expand/collapse + naming | 03 / 04 Progressive disclosure |
| Combobox | Complex input; high failure rate in wild | 03 Inputs |
| Landmarks | Page IA for AT | 05 IA / 06 A11y |
| Providing Accessible Names | Labels for controls | 07 Content / 03 Components |

## 4. Principle seeds (pre-extraction)

1. Modal dialogs must manage focus (open → into dialog; close → restore) and provide accessible name.  
2. Tabs: one tabpanel visible; keyboard per APG orientation.  
3. Every interactive control needs an accessible name (visible label preferred).

## 5. Evidence class

`Standard-adjacent Pattern Spec` — pair with WCAG for CORE elevation.

## 6. Next analysis steps

- Extract Dialog + Tabs into formal Principle cards with APG anchors  
- Compare to Carbon/Polaris modal/tabs a11y docs (Speech/Docs alignment)
