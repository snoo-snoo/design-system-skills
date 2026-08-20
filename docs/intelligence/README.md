# Design System Intelligence

Lebendes, evidenzbasiertes Design-System-Wissensmodell für AI — nicht ein Prompt-Verzeichnis.

## Grundprinzip

Jede Quelle ist zunächst **Research Material**, nicht Wahrheit.

Eine Regel wird erst **CORE**, wenn mehrere hochwertige Quellen oder starke UX-/A11y-Prinzipien sie stützen. Sonst: `EXPERIMENTAL` / `CANDIDATE`.

## Zielarchitektur

```text
SOURCE → CONTENT → ANALYSIS → RESEARCH → KNOWLEDGE → SKILL → ADAPTER → APP → VALIDATION
```

## Prioritätshierarchie (Konfliktlösung)

```text
P0 – Accessibility & Usability
… 
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
| 7 Model Adapters | ✅ | [skills/adapters/](skills/adapters/README.md) |
| 8 Validation Loop | ✅ | [validation/](validation/README.md) |

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
| [skills/adapters/](skills/adapters/README.md) | Phase-7 Model Adapters |
| [validation/](validation/README.md) | Phase-8 Validation Loop |
| [schemas/](schemas/) | Datenformate |
| [capture/](capture/) | Capture Checklists |
