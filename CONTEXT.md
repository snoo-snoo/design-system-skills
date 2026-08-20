# CONTEXT.md

## Product

**Design System Intelligence** — Pipeline und Wissensmodell, das aus öffentlichen Design-Quellen evidenzbasierte UI/UX-Regeln ableitet und daraus modellunabhängige AI Design Skills erzeugt.

## Glossary

| Term | Meaning |
| --- | --- |
| **Research Material** | Eine Quelle vor Validierung; keine automatische Wahrheit |
| **Observation** | Extrahierte Aussage oder visuelle Feststellung aus Content |
| **Principle** | Strukturierte Empfehlung mit Context/Exceptions/Evidence |
| **Canonical Rule** | Normalisierte, deduplizierte Regel nach Quality Gate |
| **CORE** | Regel mit ausreichender Evidenz für verbindliche Skills |
| **EXPERIMENTAL** | Regel mit unzureichender oder widersprüchlicher Evidenz |
| **Universal Skill** | Modellunabhängiger AI Skill; Source of Truth |
| **Model Adapter** | Plattformspezifische Hülle um einen Universal Skill |
| **Validation Loop** | Self-review + checklists + report after each skill/adapter run |
| **Speech vs Shown** | Konfliktmarkierung zwischen gesagter und gezeigter UI |
| **Wave A–D** | Themenpriorisierung für Research Sprints |

## Decisions so far

- Wave A Phases 0–8 completed (2026-08-20): Research → … → CORE Rules → Universal Skills → Model Adapters → Validation Loop.
- Adapters must not fork rules; Claude / Grok / ChatGPT profiles only change tone/shape.
- Validation: any P0 fail on `wave-a-core` → verdict `fail`.
- Social/Reels allein keine CORE-Evidence; Craft-Practices bleiben CANDIDATE.
- CX-003: Persistent labels = default; floating labels non-default.
- Token-Werte werden nicht erfunden.
- Next: Wave-B sources; optional promote CANDIDATE principles; optional runtime wiring of validation reports.

## ADR pointer

ADRs werden angelegt, wenn Architekturentscheidungen (Pipeline, Storage, Capture) verbindlich werden. Bis dahin: `docs/intelligence/research/07-research-plan.md`.
