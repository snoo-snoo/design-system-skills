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

- Phase 0–6 Wave A completed (2026-08-20): Research → Analysis → Principles → Synthesis → 7 CORE Rules → 7 Universal Skills.
- Social/Reels allein keine CORE-Evidence; Craft-Practices bleiben CANDIDATE.
- Konfliktlösung folgt P0–P7 (Accessibility vor Ästhetik).
- CX-003: Persistent labels = default (RULE-FORM-LABEL-001); floating labels non-default.
- Token-Werte werden nicht erfunden.
- Next: Phase 7 Model Adapters; Wave-B sources (Material/Atlassian, forms DS pages).

## ADR pointer

ADRs werden angelegt, wenn Architekturentscheidungen (Pipeline, Storage, Capture) verbindlich werden. Bis dahin: `docs/intelligence/research/07-research-plan.md`.
