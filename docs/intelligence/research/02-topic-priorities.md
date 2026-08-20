# Themenpriorisierung (Phase 0)

Welche Design-System-Themen zuerst erforscht werden — vor Content-Analyse und Skill-Generierung.

## Wave A — Foundations mit hoher Übertragbarkeit

Diese Themen erzeugen die meisten wiederverwendbaren Regeln und blockieren später kaum.

| Priorität | Thema | Warum zuerst |
| --- | --- | --- |
| A1 | Accessibility Foundations | P0-Konfliktlösung; WCAG als Evidenzanker |
| A2 | Typography System | Hierarchie, Lesbarkeit, Content Density |
| A3 | Spacing & Layout Rhythm | Konsistenz über Komponenten hinweg |
| A4 | Color Semantics & Contrast | Modes, Status, Action Emphasis |
| A5 | Focus, Keyboard, Touch Targets | Interaktions-Zugänglichkeit |

## Wave B — Hochfrequente Komponenten & Patterns

| Priorität | Thema | Warum |
| --- | --- | --- |
| B1 | Buttons & Action Hierarchy | Primär vs Sekundär vs Destructive |
| B2 | Forms & Validation | Häufigste Product-UI; Error Prevention |
| B3 | Navigation & IA | Globale Orientierungsregeln |
| B4 | Feedback States | Empty / Loading / Error / Success |
| B5 | Modals, Dialogs, Overlays | Fokus-Fallen, Dismissal, Hierarchy Risks |

## Wave C — Product Surfaces

| Priorität | Thema | Warum später |
| --- | --- | --- |
| C1 | Tables & Data Density | Stark kontextabhängig (Enterprise) |
| C2 | Dashboards | Viele konkurrierende Heuristiken |
| C3 | Onboarding & Auth | Content + Flow + Security Constraints |
| C4 | Search & Filtering | Pattern-Varianz hoch |
| C5 | Checkout / Commerce | Branchenspezifisch |

## Wave D — Emerging / AI UI

| Priorität | Thema | Hinweis |
| --- | --- | --- |
| D1 | AI Chat & Streaming States | Schnell wandelnd → zunächst EXPERIMENTAL |
| D2 | Copilot / Agent UX | Human-in-the-loop, Citations |
| D3 | Generative UI | Hohe Unsicherheit; starke Validierung nötig |
| D4 | Confidence & Uncertainty UI | Evidenz noch dünn |

## Explizit nachrangig in Phase 0–2

- Brand-heavy Marketing Visuals als „universelle“ Rules
- Einzelne Aesthetic Trends (Glassmorphism, Neumorphism, etc.)
- Tooling-only Ratschläge ohne UI-Wirkung (reine Figma Shortcuts)
- Creator-Persönlichkeits-Workflows ohne übertragbares Prinzip

## Erfolgsmaßstab für Themenreife

Ein Thema darf in **Canonical Rules** übergehen, wenn:

1. ≥ 3 unabhängige Qualitätsquellen ODER 1 starker Standard (z. B. WCAG)
2. Klare Recommendation + Context + Exceptions
3. Mindestens 1 Anti-Pattern
4. AI-anwendbar und validierbar
5. Kein ungelöster P0-Konflikt mit Accessibility
