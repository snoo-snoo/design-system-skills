# CONTEXT.md

## Product

**Design System Intelligence** — Pipeline und Wissensmodell, das aus öffentlichen Design-Quellen evidenzbasierte UI/UX-Regeln ableitet und daraus modellunabhängige AI Design Skills erzeugt.

## Glossary

| Term | Meaning |
| --- | --- |
| **Research Material** | Eine Quelle vor Validierung; keine automatische Wahrheit |
| **Principle** | Strukturierte Empfehlung mit Context/Exceptions/Evidence |
| **Canonical Rule** | Normalisierte Regel nach Quality Gate |
| **CORE** | Regel mit ausreichender Evidenz für verbindliche Skills |
| **Universal Skill** | Modellunabhängiger AI Skill; Source of Truth |
| **Model Adapter** | Plattformspezifische Hülle um einen Universal Skill |
| **Validation Loop** | Self-review + checklists + report after each run |
| **Wave A–D** | Themenpriorisierung für Research Sprints |

## Decisions so far

- Wave A Phases 0–8 complete; Wave B pass complete (2026-08-20).
- **11 CORE rules** / **11 Universal Skills** / adapters for Claude·Grok·ChatGPT.
- Wave B promotions: radius scale, color restraint, form feedback, action hierarchy.
- Still held: nested radius, text-align, border restraint, API parity, card surface.
- CX-006: prefer validation over silent disabled primary — not a blanket ban.
- Token values are never invented.
- Next: deepen Wave B (buttons across more DS, navigation) or Wave C product surfaces.

## ADR pointer

`docs/intelligence/research/07-research-plan.md`
