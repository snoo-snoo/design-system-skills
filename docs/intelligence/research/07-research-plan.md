# Research-Plan — Phases 0–6

**Status:** Phase 0–6 Wave A ✅ (2026-08-20) · Phase 7–8 geplant  
**Nächster Schritt:** Wave-B Quellen (Material/Atlassian, Forms DS pages) · Phase 7 Model Adapters

## Ziel

Aus öffentlichen Design-Ressourcen belastbare Principles und Canonical Rules gewinnen und daraus atomare Universal Skills ableiten — ohne Meinungen zu automatischen Regeln zu erklären.

## Scope Freeze (durch Wave A)

In Scope (geliefert):

- Foundations, Accessibility, Core Components (Dialog/Tabs), Forms labels
- Evidenz aus Design Systems, Standards, Heuristics, kuratierten Videos
- Schema-ready Artifacts → CORE Rules → Universal Skills

Out of Scope (noch):

- Model Adapters (Phase 7)
- Validation Loop Automation (Phase 8)
- Automatisierte Instagram-Scraping-Pipeline
- Token-Zahlen erfinden
- Brand/Marketing-Ästhetik als universelle Product-UI-Rules

---

## Arbeitspakete

### WP0 — Taxonomy & Schemas ✅

- [x] Taxonomie, Waves, Experten, Quellen, DS Matrix, Standards, Schemas

### WP1 — Source Indexing ✅

- [x] Source Profiles + Capture checklists + Contradiction log stub

### WP2 — Content Analysis ✅ (Wave A sample set)

- [x] ST-001/002/003 maps · DS-002/003/005 · VID-SAMPLE-001…007

### WP3 — Principle Extraction ✅

- [x] Principle cards under `docs/intelligence/principles/`

### WP4 — Cross-Source Synthesis ✅

- [x] [`docs/intelligence/synthesis/wave-a.md`](../synthesis/wave-a.md)
- [x] Consensus / contradictions / context splits / emerging patterns

### WP5 — Canonical Rules ✅ (Wave A CORE batch)

- [x] [`docs/intelligence/rules/`](../rules/README.md) — 7 CORE rules

### WP6 — Atomic Universal Skills ✅ (from CORE only)

- [x] [`docs/intelligence/skills/universal/`](../skills/README.md) — 7 skills

### WP7 — Model Adapters (next)

- [ ] Claude / Grok / ChatGPT wrappers; no forked rule content

### WP8 — Validation Loop (later)

- [ ] Self-review checklists wired into application flows

---

## Wave A CORE batch

| Rule | Skill |
| --- | --- |
| RULE-FOCUS-001 | ensure-visible-focus |
| RULE-TOUCH-001 | size-touch-targets |
| RULE-FORM-LABEL-001 | label-form-fields |
| RULE-DIALOG-001 | build-accessible-modal |
| RULE-TABS-001 | build-accessible-tabs |
| RULE-SPACE-001 | apply-spacing-scale |
| RULE-COLOR-001 | apply-semantic-color |

CANDIDATE (no skill yet): RADIUS-*, COLOR-RESTRAINT, TEXT-ALIGN, BORDER-RESTRAINT, FORM-FEEDBACK, COMPONENT-API-PARITY  
EXPERIMENTAL: CARD-SURFACE-001

---

## Methodenregeln (verbindlich)

1. Eine Designer-Aussage ≠ Regel.
2. Confidence steigt nur mit Evidence Mix.
3. Bei Konflikt: P0–P7 Hierarchie; keine Fake-Consensus.
4. Keine exakten Token-Werte ohne belastbare Quelle.
5. Jede Normalisierung muss Originalaussage referenzieren.
6. Rules dürfen sich durch neue Evidenz ändern — Changelog führen.
7. Skills nur aus CORE Rules; ein Skill = eine Aufgabe.

---

## Repo-Layout

```text
docs/intelligence/
├── research/                 ← Phase 0
├── schemas/
├── sources/                  ← Phase 1
├── analysis/                 ← Phase 2
├── principles/               ← Phase 3
├── synthesis/                ← Phase 4
├── rules/                    ← Phase 5
├── skills/                   ← Phase 6
│   └── universal/
│   └── adapters/             ← Phase 7 (pending)
└── capture/
```

---

## Definition of Done — Wave A (Phases 0–6)

- [x] Taxonomy & evidence model
- [x] Indexed sources + analyses for Wave A set
- [x] Principles extracted
- [x] Cross-source synthesis written
- [x] CORE Canonical Rules gated
- [x] Universal Skills for each CORE rule
- [ ] Model adapters
- [ ] Automated validation loop
