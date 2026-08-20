# Design System Intelligence

Lebendes, evidenzbasiertes Design-System-Wissensmodell für AI — nicht ein Prompt-Verzeichnis.

## Grundprinzip

Jede Quelle ist zunächst **Research Material**, nicht Wahrheit.

Strikte Trennung von:

| Klasse | Beispiel |
| --- | --- |
| Persönliche Meinung | „Ich mag Rounded Corners“ |
| Subjektiver Geschmack | „Neon ist modern“ |
| Persönlicher Workflow | „Ich starte immer in Figma Auto Layout“ |
| Empirische Best Practice | „Touch Targets ≥ 44×44 px verbessern Fehlerraten“ |
| Usability-Prinzip | Nielsen Heuristics, Cognitive Load |
| Accessibility-Anforderung | WCAG 2.2 Contrast / Focus |
| Design-System-Konvention | Semantic Tokens, Composition |
| Plattformkonvention | Apple HIG / Material Navigation |
| Technische Einschränkung | CSS Cascade, Native Controls |
| Visuelle Präferenz | Brand Expression |
| Wissenschaftlich belegtes Prinzip | Fitts’s Law, Hick’s Law |

Eine Regel wird erst **CORE**, wenn mehrere hochwertige Quellen oder starke UX-/A11y-Prinzipien sie stützen. Sonst: `EXPERIMENTAL` / `CANDIDATE`.

## Zielarchitektur

```text
SOURCE → CONTENT → ANALYSIS → RESEARCH → KNOWLEDGE → SKILL → ADAPTER → APP → VALIDATION
```

## Prioritätshierarchie (Konfliktlösung)

```text
P0 – Accessibility & Usability
P1 – Functional clarity
P2 – Information hierarchy
P3 – Interaction consistency
P4 – Design-system consistency
P5 – Visual hierarchy
P6 – Brand expression
P7 – Aesthetic preferences
```

## Phasen

| Phase | Status | Output |
| --- | --- | --- |
| 0 Research & Taxonomy | ✅ | Themen, Quellen, Plan |
| 1 Source Indexing | ✅ | Source Profiles |
| 2 Content Analysis | ✅ Wave A | Transcripts, Visual Notes |
| 3 Principle Extraction | ✅ | Principles + Confidence |
| 4 Cross-Source Synthesis | ✅ | [synthesis/wave-a.md](synthesis/wave-a.md) |
| 5 Canonical Rules | ✅ | [rules/](rules/README.md) (7 CORE) |
| 6 Atomic Skills | ✅ | [skills/universal/](skills/README.md) |
| 7 Model Adapters | Geplant | Claude / Grok / ChatGPT |
| 8 Validation Loop | Geplant | Self-Review Checklists |

## Einstiege

| Datei | Inhalt |
| --- | --- |
| [research/](research/) | Phase-0 Taxonomy & Plan |
| [sources/](sources/README.md) | Phase-1 Source Index |
| [analysis/](analysis/README.md) | Phase-2 Analysis Index |
| [principles/](principles/) | Phase-3 Principles |
| [synthesis/](synthesis/README.md) | Phase-4 Synthesis |
| [rules/](rules/README.md) | Phase-5 Canonical Rules |
| [skills/](skills/README.md) | Phase-6 Universal Skills |
| [schemas/](schemas/) | Datenformate |
| [capture/](capture/) | Capture Checklists |
