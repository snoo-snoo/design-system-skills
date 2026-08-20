# Research-Plan — Phases 0–8

**Status:** Wave A Phases 0–8 ✅ (2026-08-20)  
**Nächster Schritt:** Wave-B Quellen (Material/Atlassian, Forms DS pages) · promote CANDIDATE principles when evidence allows

## Ziel

Aus öffentlichen Design-Ressourcen belastbare Principles und Canonical Rules gewinnen, daraus atomare Universal Skills ableiten, modellspezifisch wrappen und validieren — ohne Meinungen zu automatischen Regeln zu erklären.

## Scope Freeze (Wave A complete)

In Scope (geliefert):

- Foundations, Accessibility, Core Components (Dialog/Tabs), Forms labels
- Evidenz → Principles → Synthesis → CORE Rules → Universal Skills
- Model Adapters (Claude / Grok / ChatGPT)
- Validation Loop + checklists + report schema

Out of Scope (noch):

- Automatisierte Instagram-Scraping-Pipeline
- Token-Zahlen erfinden
- Brand/Marketing-Ästhetik als universelle Product-UI-Rules
- Runtime app automation (docs-level loop only for now)

---

## Arbeitspakete

### WP0–WP6 ✅

Research → Indexing → Analysis → Principles → Synthesis → CORE Rules → Universal Skills

### WP7 — Model Adapters ✅

- [x] Adapter schema + contract (no forked rules)
- [x] Profiles: Claude, Grok, ChatGPT
- [x] Thin skill adapters for all 7 Universal Skills
- [x] Shared invoke template + validation hook

**Deliverable:** [`docs/intelligence/skills/adapters/`](../skills/adapters/README.md)

### WP8 — Validation Loop ✅

- [x] Loop process (`validation/loop.md`)
- [x] Checklists: wave-a-core, accessibility, consistency, ux, design-system
- [x] Report schema + template + example
- [x] P0 fail = block verdict

**Deliverable:** [`docs/intelligence/validation/`](../validation/README.md)

---

## Wave A CORE batch

| Rule | Skill | Adapters |
| --- | --- | --- |
| RULE-FOCUS-001 | ensure-visible-focus | claude / grok / chatgpt |
| RULE-TOUCH-001 | size-touch-targets | claude / grok / chatgpt |
| RULE-FORM-LABEL-001 | label-form-fields | claude / grok / chatgpt |
| RULE-DIALOG-001 | build-accessible-modal | claude / grok / chatgpt |
| RULE-TABS-001 | build-accessible-tabs | claude / grok / chatgpt |
| RULE-SPACE-001 | apply-spacing-scale | claude / grok / chatgpt |
| RULE-COLOR-001 | apply-semantic-color | claude / grok / chatgpt |

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
8. Adapters forken keine Rules; Validation Loop nach jedem Run.

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
├── skills/                   ← Phase 6–7
│   ├── universal/
│   └── adapters/
└── validation/               ← Phase 8
```

---

## Definition of Done — Wave A (Phases 0–8)

- [x] Taxonomy & evidence model
- [x] Indexed sources + analyses
- [x] Principles + synthesis
- [x] CORE Canonical Rules
- [x] Universal Skills
- [x] Model adapters (Claude / Grok / ChatGPT)
- [x] Validation loop + checklists + report template
