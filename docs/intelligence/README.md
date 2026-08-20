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

Eine Regel wird erst **CORE**, wenn mehrere hochwertige Quellen oder starke UX-/A11y-Prinzipien sie stützen. Sonst: `EXPERIMENTAL`.

## Zielarchitektur

```text
SOURCE LAYER
Instagram / YouTube / Articles / Design Systems
        ↓
CONTENT LAYER
Videos / Audio / Images / Text
        ↓
ANALYSIS LAYER
Transcription / Vision / NLP
        ↓
RESEARCH LAYER
Observations / Principles / Evidence
        ↓
KNOWLEDGE LAYER
Canonical Rules / Patterns / Taxonomy
        ↓
SKILL LAYER
Atomic AI Design Skills
        ↓
MODEL ADAPTER
Claude / Grok / ChatGPT / Other
        ↓
APPLICATION
UI Generation / UX Review / Design Audit
        ↓
VALIDATION
Consistency / Accessibility / UX / Design System
```

## Knowledge Graph (Ziel)

```text
Creator → Content → Observation → Principle → Rule
  → Pattern → Component → Design Skill → Validation Rule
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
| 0 Research & Taxonomy | **Aktiv** | Themen, Quellen, Plan |
| 1 Source Indexing | Geplant | Source Profiles |
| 2 Content Analysis | Geplant | Transcripts, Visual Notes |
| 3 Principle Extraction | Geplant | Principles + Confidence |
| 4 Cross-Source Synthesis | Geplant | Consensus / Contradictions |
| 5 Canonical Rules | Geplant | RULE-xxx Library |
| 6 Atomic Skills | Geplant | Universal Skills |
| 7 Model Adapters | Geplant | Claude / Grok / ChatGPT |
| 8 Validation Loop | Geplant | Self-Review Checklists |

## Dokumente (Phase 0)

| Datei | Inhalt |
| --- | --- |
| [research/01-taxonomy.md](research/01-taxonomy.md) | Standard-Taxonomie |
| [research/02-topic-priorities.md](research/02-topic-priorities.md) | Themenpriorisierung |
| [research/03-experts-creators.md](research/03-experts-creators.md) | Experten & Creator |
| [research/04-sources-catalog.md](research/04-sources-catalog.md) | Quellenkatalog |
| [research/05-design-systems.md](research/05-design-systems.md) | Design-Systeme |
| [research/06-standards-evidence.md](research/06-standards-evidence.md) | Standards & Evidenz |
| [research/07-research-plan.md](research/07-research-plan.md) | Research-Plan |
| [schemas/](schemas/) | Datenformate für spätere Phasen |
