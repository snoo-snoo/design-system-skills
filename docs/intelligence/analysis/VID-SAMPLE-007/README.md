# Analysis — VID-SAMPLE-007 (Design–Code Component Parity)

**Source:** [VID-SAMPLE-007](../../sources/VID-SAMPLE-007.md) · **Captured:** 2026-08-20

## 1. Source Summary

Educator Reel: don’t design components without understanding code. Designers can author Figma component props but often don’t know how those props map in React — a common reason design systems break.

## 2. Capture limits

Caption ✅ · Full transcript ❌ · Visuals partial (cover; likely shows Figma props ↔ React) · `SpeechVsVisual: partial` · DM “React prop guide” not captured

## 3. Claims

| ID | Statement | Class | Confidence |
| --- | --- | --- | --- |
| C1 | Many designers can build Figma props but don’t understand React prop behavior | Observation / Opinion | Medium |
| C2 | That gap causes design systems to break | Practice / Assertion | Medium–High |
| C3 | Designers should not design components “without code” (without implementation literacy) | Practice / Workflow | Medium–High |
| C4 | Learning React prop mapping improves DS reliability | Practice | Medium |

## 4. Classification notes

- Not a visual UI rule (color/spacing/layout) — **design-system architecture / process**
- Framework-specific wording (React) → generalize to “implementation API”
- Does not require every designer to write production code; requires shared prop contract literacy

## 5. Cross-source

- Aligns with Primer/Carbon/Polaris treating systems as engineering products (versioned APIs, tokens)
- Complements token discipline (COLOR/SPACE): props are another contract layer
- Related future skill: `design-system-audit` / component API review

## 6. Principle

→ [PRINCIPLE-COMPONENT-API-PARITY-001](../../principles/PRINCIPLE-COMPONENT-API-PARITY-001.md) (CANDIDATE)

## 7. Anti-pattern

Inventing Figma variants/props that cannot be expressed (or are inconsistently expressed) in the coded component API — drifting design and engineering sources of truth.
