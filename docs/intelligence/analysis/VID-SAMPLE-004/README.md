# Analysis — VID-SAMPLE-004 (Revolut Form Principles)

**Source:** [VID-SAMPLE-004](../../sources/VID-SAMPLE-004.md) · **Captured:** 2026-08-20

## 1. Source Summary

Breakdown of Revolut-style form craft: reduce effort, build confidence, keep momentum. LinkedIn cross-post lists six principles. Strong accessibility debate in comments.

## 2. Capture limits

Caption ✅ · Six principles via LinkedIn comments ✅ · Full demo frames ❌ · `SpeechVsVisual: partial`

## 3. Stated “Revolut” principles (from LinkedIn)

1. **Floating labels** — label never disappears / adaptive inputs  
2. **Touch targets** — generous, thumb-friendly  
3. **Rounded corners** — softer containers feel approachable  
4. **Spatial continuity** — fluid transitions across multi-step flows  
5. **Active state animation** — immediate interaction feedback  
6. **CTA evolution** — primary action changes with progress

## 4. Claim classification

| Principle | Class | Confidence | Notes |
| --- | --- | --- | --- |
| Touch targets | Practice + Standard-adjacent | **High** | Aligns WCAG 2.5.8 / PRINCIPLE-FOCUS sizing |
| Spatial continuity | Practice | Medium | Good UX narrative; needs pattern evidence |
| Active state feedback | Heuristic (#1 status) | High as idea | Respect `prefers-reduced-motion` |
| CTA evolution | Practice | Medium | Progress-aware CTAs; don’t hide destructive clarity |
| Rounded corners | Taste / Practice | Low–Medium | Aesthetic; not a11y |
| Floating labels | Contested Practice | **Low for CORE** | Heavy expert a11y pushback |

## 5. Conflicts (CX-003)

Floating labels vs persistent labels:

- Pros claimed: save space, label remains in some form  
- Cons (commenters / a11y practitioners): looks prefilled; tiny active label; zoom/reflow issues; motion sensitivity; localization; better pattern = persistent label above field

**Decision rule:** P0 Accessibility → prefer persistent visible labels as default CORE path. Floating labels = EXPERIMENTAL / context-only.

## 6. Principles spawned

- [PRINCIPLE-TOUCH-TARGET-001](../../principles/PRINCIPLE-TOUCH-TARGET-001.md) — CANDIDATE/CORE-ready  
- [PRINCIPLE-FORM-LABEL-001](../../principles/PRINCIPLE-FORM-LABEL-001.md) — persistent labels (from conflict resolution)  
- [PRINCIPLE-FORM-FEEDBACK-001](../../principles/PRINCIPLE-FORM-FEEDBACK-001.md) — immediate field/system feedback  
- Floating-label tip retained only as EXPERIMENTAL observation in claims (not promoted)

## 7. Anti-patterns

- Placeholder-as-only-label  
- Tiny hit areas on mobile money actions  
- Motion-only feedback without reduced-motion alternative
