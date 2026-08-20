# Wave A — Cross-Source Synthesis

**Date:** 2026-08-20  
**Scope:** Foundations (space, color, radius), Accessibility (focus, targets, labels), Core components (dialog, tabs), Forms feedback, selected social Practices  
**Inputs:** ST-001/002/003 analysis maps · DS-002/003/005 foundations · PRINCIPLE-* cards · VID-SAMPLE-001…007 · [_contradictions.md](_contradictions.md)

---

## 1. Consensus (promote toward CORE)

Patterns with **independent Standard and/or multi-system** support. These pass or nearly pass the Phase-5 Quality Gate.

| Theme | Consensus statement | Evidence mix | Principle → Rule |
| --- | --- | --- | --- |
| Focus visibility | Interactive controls must show a visible, unobscured focus indicator; focus order matches the interaction model | WCAG 2.4.7 / 2.4.11 + Carbon/Primer focus tokens + APG dialog notes | FOCUS-001 → **RULE-FOCUS-001** |
| Touch targets | Pointer targets must meet accessibility minimums; padding may enlarge hit area | WCAG 2.5.8 + Primer control sizes + VID-004 practice | TOUCH-TARGET-001 → **RULE-TOUCH-001** |
| Persistent labels | Form fields keep a persistent visible label; placeholder-only / disappearing labels are non-default | WCAG 3.3.2 direction + a11y critique of floating labels (CX-003) | FORM-LABEL-001 → **RULE-FORM-LABEL-001** |
| Modal dialog a11y | Modals are named, focus-trapped, Esc-dismissible, restore focus | APG Dialog + WCAG operable + Heuristics #1/#3 | DIALOG-001 → **RULE-DIALOG-001** |
| Tabs semantics | Tabs use tablist/tab/tabpanel roles, one selected tab, arrow-key navigation | APG Tabs + Heuristics #4/#6 | TABS-001 → **RULE-TABS-001** |
| Spacing scale | Layout/component space uses a discrete token scale, not ad-hoc px | Carbon Spacing + Primer size/stack (+ Polaris card padding) | SPACE-001 → **RULE-SPACE-001** |
| Semantic color | Product color goes through role-based tokens/themes, not raw hex | Carbon Color + DS matrix token APIs | COLOR-001 → **RULE-COLOR-001** |

**Quality note:** FOCUS and TOUCH were already CORE-ready. FORM-LABEL, DIALOG, TABS, SPACE, COLOR are elevated to CORE in this Wave-A gate pass based on synthesis above (Standards + ≥1 system or strong a11y pattern docs).

---

## 2. Strong Practices (remain CANDIDATE)

Useful for guidance and future skills, but **not** CORE yet — social-heavy or single-system craft without Standard floor.

| Theme | Statement | Why not CORE | Principle |
| --- | --- | --- | --- |
| Nested radius | `outer = inner + padding` for concentric nesting | Practice + educator corpus; DS use fixed token scales (CX-001 complementary) | RADIUS-001 |
| Radius scale | Prefer semantic radius tokens (sm/md/lg/full) | System convention; needs Material/Atlassian quote for broader consensus | RADIUS-SCALE-001 |
| Color restraint | Limit decorative color; reserve strong color for meaning | Aligns with Carbon “sparingly” but primarily craft/Reel evidence | COLOR-RESTRAINT-001 |
| Text alignment | Prefer start alignment for multi-line UI text | Strong craft; limited Standard/DS formalization | TEXT-ALIGN-001 |
| Border restraint | Prefer whitespace over dense decorative borders | Craft + SPACE proximity; exceptions protect P0 borders | BORDER-RESTRAINT-001 |
| Form feedback | Immediate visible feedback for focus/validation/progress | Heuristic + Reel practice; needs DS form-pattern cross-check | FORM-FEEDBACK-001 |
| API parity | Design props map to implementation component API | DS governance practice; not yet multi-doc formalized | COMPONENT-API-PARITY-001 |

---

## 3. Emerging / contested (EXPERIMENTAL or resolved non-default)

| Theme | Status | Resolution |
| --- | --- | --- |
| Borderless / chrome-light cards | EXPERIMENTAL (CARD-SURFACE-001) | CX-004 open — P0 contrast/readability overrides aesthetics |
| Floating labels as default | Rejected as default | CX-003 → persistent labels CORE; floating = brand exception only |
| Nested radius as system law | Not elevated | CX-001 complementary composition tip on top of tokens |

---

## 4. Contextual differences (do not fake consensus)

| Topic | Context A | Context B | Handling |
| --- | --- | --- | --- |
| Color density | Product UI / admin → restrained neutrals | Marketing / brand campaigns → expressive color allowed | COLOR-RESTRAINT scoped; COLOR tokens still apply where system exists |
| Borders | Content layouts → space-first | Tables, inputs, focus, high-density tools → borders often required | BORDER-RESTRAINT exceptions; P0 wins |
| Radius nesting | Optical craft on custom surfaces | Tokenized systems (Primer/Polaris) → pick nearest tokens | Complementary guidance |
| Platform dialogs | Web APG pattern | Native `<dialog>` / HIG sheets | Same outcomes, different APIs — document as equivalent behaviors |
| Text alignment | Product body copy → start | Hero/empty-state short titles → center OK | TEXT-ALIGN exceptions |
| Touch size | WCAG minimum | Comfortable mobile primary actions (fintech) | Minimum = MUST; comfort = SHOULD |

---

## 5. Contradiction rollup

See [_contradictions.md](_contradictions.md).

| ID | Synthesis outcome |
| --- | --- |
| CX-001 | Complementary — no CORE conflict |
| CX-002 | Open — do not elevate disabled-contrast claims |
| CX-003 | Resolved for defaults — RULE-FORM-LABEL-001 |
| CX-004 | Open — CARD-SURFACE stays EXPERIMENTAL |
| CX-005 | Noted — covered by BORDER-RESTRAINT exceptions |

---

## 6. Priority hierarchy applied

When craft advice conflicts with accessibility:

1. **P0** wins (focus rings, target size, labels, dialog traps, contrast) over borderless chrome, floating labels, decorative restraint.
2. **P4** system tokens (space/color/radius scales) win over one-off social “tips” that invent values.
3. **P5–P7** craft (nested radius, alignment, border aesthetics) may become SHOULD skills later — never override P0–P3.

---

## 7. Wave-A CORE batch (Phase 5 input)

Promote now:

1. RULE-FOCUS-001  
2. RULE-TOUCH-001  
3. RULE-FORM-LABEL-001  
4. RULE-DIALOG-001  
5. RULE-TABS-001  
6. RULE-SPACE-001  
7. RULE-COLOR-001  

Hold as CANDIDATE (no Universal Skill yet): RADIUS-*, COLOR-RESTRAINT, TEXT-ALIGN, BORDER-RESTRAINT, FORM-FEEDBACK, COMPONENT-API-PARITY.

Hold as EXPERIMENTAL: CARD-SURFACE-001.

---

## 8. Gaps for Wave B

- Material 3 / Atlassian foundations pages → harden SPACE/COLOR/RADIUS-SCALE  
- Carbon/Polaris modal a11y pages → optional second cite for DIALOG  
- CX-002 Carbon disabled contrast deep-dive  
- Forms pattern pages across Polaris/Carbon → FORM-FEEDBACK CORE path  
- Non-social conference talks for craft practices (radius, alignment)

---

## Definition of Done — Phase 4 (Wave A)

- [x] Consensus table with evidence mix  
- [x] Contradictions referenced and default resolutions recorded  
- [x] Context splits documented  
- [x] Emerging patterns kept non-CORE  
- [x] Explicit CORE candidate list for Phase 5  
- [x] No skills generated in this phase artifact  
