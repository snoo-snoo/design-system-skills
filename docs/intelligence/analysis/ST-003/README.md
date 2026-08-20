# Analysis Report — ST-003 (NN/g 10 Usability Heuristics)

**Source:** [ST-003](../../sources/ST-003.md)  
**Captured:** 2026-08-20  
**Status:** `in_analysis`

## 1. Source Summary

Ten interaction-design heuristics (Nielsen; refined 1994; article updated 2020). Broad rules of thumb — not component specs.

## 2. Heuristic → Taxonomy map

| # | Heuristic | Primary taxonomy | Wave |
| --- | --- | --- | --- |
| 1 | Visibility of system status | 04 Feedback / Loading / 09 AI States | A |
| 2 | Match system–real world | 07 Content / 05 UX | A |
| 3 | User control and freedom | 05 UX / Modals / Undo | A |
| 4 | Consistency and standards | 04 DS consistency / Platforms | A |
| 5 | Error prevention | 04 Forms / 05 Error Prevention | B |
| 6 | Recognition rather than recall | 05 UX / Navigation | A |
| 7 | Flexibility and efficiency | 05 UX / Shortcuts | B |
| 8 | Aesthetic and minimalist design | 02 Hierarchy / Content priority | A |
| 9 | Recognize, diagnose, recover from errors | 04 Error States / 07 Microcopy | A |
| 10 | Help and documentation | 07 Content | B |

## 3. Caution flags

- Heuristic #8 ≠ “remove enterprise density” or “flat design only”
- Heuristics alone → max **CANDIDATE** for component specifics; need systems/WCAG for CORE
- Aesthetic tips (VID-SAMPLE-001) may support #4/#8 craft but stay P5

## 4. Principle seeds

1. Continuous status feedback for async/AI operations (ties to 09 AI UI)  
2. Errors: plain language + cause + next step (#9)  
3. Destructive flows: escape/cancel/undo (#3 + #5)

## 5. Next analysis steps

- Pair #1/#9 with Polaris/Carbon banner/toast/form-error docs  
- Pair #3 with APG Dialog dismiss patterns
