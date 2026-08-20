# Analysis — VID-SAMPLE-005 (Centered Multi-line Text)

**Source:** [VID-SAMPLE-005](../../sources/VID-SAMPLE-005.md) · **Captured:** 2026-08-20

## 1. Source Summary

Claims stacking multiple lines of center-aligned text creates too many alignment anchors; designers should stop centering text in UI by default.

## 2. Capture limits

Caption ✅ · Full transcript ❌ · Visuals partial · `SpeechVsVisual: partial`

## 3. Claims

| ID | Statement | Class | Confidence |
| --- | --- | --- | --- |
| C1 | Multi-line centered text creates too many alignment anchors | Practice | Medium–High |
| C2 | Default to non-centered (typically start/left) alignment for UI text blocks | Practice | Medium–High |
| C3 | Centering text in UI is a common designer mistake | Opinion | Medium |

## 4. Exceptions (implied / standard craft)

- Short headlines, hero statements, empty-state titles  
- Single-line CTAs / captions  
- Centered layouts that are intentional brand moments with limited line count

## 5. Cross-source

Classic typography/layout craft; supports hierarchy/scanability (NN/g recognition, content design). No WCAG prohibition of centered text, but long centered body harms readability.

## 6. Principle

→ [PRINCIPLE-TEXT-ALIGN-001](../../principles/PRINCIPLE-TEXT-ALIGN-001.md) (CANDIDATE)

## 7. Anti-pattern

Multi-paragraph or multi-line body/UI copy centered, producing ragged left+right edges and weak vertical rhythm.
