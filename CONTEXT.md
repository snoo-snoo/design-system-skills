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
| **Speech vs Shown** | Konfliktmarkierung zwischen gesagter und gezeigter UI |
| **Wave A–D** | Themenpriorisierung für Research Sprints |

## Decisions so far

- Phase 0 vor Skill-Generierung (Research & Taxonomy first).
- Phase 1 Source Indexing completed (profiles in `docs/intelligence/sources/`).
- Social/Reels sind indexierbar, aber allein keine CORE-Evidence.
- Konfliktlösung folgt P0–P7 (Accessibility vor Ästhetik).
- Token-Werte werden nicht erfunden.
- Phase 2 batch: VID-SAMPLE-002…005 analyzed; form floating-label conflict documented (CX-003); touch-target + persistent-label principles added.
- Next: first Canonical Rules from FOCUS-001 and TOUCH-TARGET-001.

## ADR pointer

ADRs werden angelegt, wenn Architekturentscheidungen (Pipeline, Storage, Capture) verbindlich werden. Bis dahin: `docs/intelligence/research/07-research-plan.md`.
