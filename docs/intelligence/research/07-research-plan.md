# Research-Plan — Phase 0 → Phase 2

**Status:** Phase 0 ✅ · Phase 1 ✅ · Phase 2 **in progress** (sample Reel + Wave A docs started).  
**Nächster Schritt:** Foundations deep-dives (Carbon/Polaris/Primer) + APG Dialog/Tabs principle cards — noch **keine** Skill-Generierung.

## Ziel dieser Phase

Ein wiederholbarer Plan, um aus öffentlichen Design-Ressourcen belastbare Principles und später Canonical Rules zu gewinnen — ohne Meinungen zu automatischen Regeln zu erklären.

## Scope Freeze (bis Phase 5)

In Scope:

- Foundations, Accessibility, Core Components, Feedback States, Forms
- Evidenz aus Design Systems, Standards, Research Orgs, kuratierten Videos
- Schema-ready Research Artifacts

Out of Scope (vorerst):

- Fertige AI Skills / Model Adapter
- Automatisierte Instagram-Scraping-Pipeline
- Token-Zahlen erfinden
- Brand/Marketing-Ästhetik als universelle Product-UI-Rules

---

## Arbeitspakete

### WP0 — Taxonomy & Schemas ✅

- [x] Taxonomie (01 Foundations … 09 AI UI)
- [x] Themenpriorisierung Wave A–D
- [x] Experten-/Quellenkatalog (Seed)
- [x] Design-System Study Matrix
- [x] Standards & Evidence Mapping
- [x] Schemas für Source / Principle / Rule / Skill

### WP1 — Source Indexing ✅

Für jede Seed-Quelle in `04-sources-catalog.md`:

1. Source Profile anlegen (`schemas/source-profile.md`)
2. Expertise / Credibility / Relevance bewerten
3. Primäre Themen-Tags (Taxonomie) setzen
4. Capture-Methode festlegen (Docs scrape / Video transcript / Manual notes)
5. Status: `queued | indexed | in_analysis | analyzed | blocked`

**Reihenfolge:** ST-* und DS-* vor VID-* und Social.

**Deliverable:** [`docs/intelligence/sources/`](../sources/README.md) — Kickoff-Set indexed; weitere Seeds queued/indexed.

**Erledigt (2026-08-20):**

- Capture checklists: docs + video
- Indexed: ST-001–003, DS-001/002/003/004/005/008, RE-001, RE-004
- Queued thin profiles: remaining DS/ST/RE/VID seeds
- Contradiction log stub vorhanden

### WP2 — Content Analysis (in progress)

Pro Content Unit:

1. Transkript / Text extract
2. Visual observations (wenn Video/UI)
3. Speech vs Shown Konflikte markieren
4. Claim inventory (Recommendation / Assertion / Example / Caveat)
5. Statement class: Opinion | Taste | Workflow | Practice | Principle | Standard | Constraint

**Startreihenfolge:** ST-001 → ST-002 → ST-003 → DS-002 / DS-003 / DS-005 Foundations pages (+ sample social video).

**Deliverable:** [`docs/intelligence/analysis/`](../analysis/README.md)

**Erledigt (2026-08-20):**

- Sample Instagram Reel `VID-SAMPLE-001` fully pipeline-tested (partial visuals)
- Principle `PRINCIPLE-RADIUS-001` → CANDIDATE after DS cross-check
- ST-001 / ST-002 / ST-003 analysis kickoff maps
- DS-002 / DS-003 / DS-005 Foundations claim inventories
- APG-derived PRINCIPLE-DIALOG-001 + PRINCIPLE-TABS-001
- SPACE / COLOR / FOCUS / RADIUS-SCALE principle candidates
- CX-001 resolved as complementary

### WP3 — Principle Extraction

Claims → Principle Cards (`schemas/principle.md`) mit Confidence vorläufig **nur lokal** (noch nicht CORE).

### WP4 — Cross-Source Synthesis

- Common Patterns
- Consensus
- Contradictions
- Contextual Differences
- Emerging Patterns (default EXPERIMENTAL)

**Deliverable:** `docs/intelligence/synthesis/wave-a.md`

### WP5 — Canonical Rules (Quality Gate)

Nur Rules, die das Quality Gate bestehen → `docs/intelligence/rules/RULE-xxx.md`

Quality Gate:

- Klar, wiederverwendbar, kontextuiert
- Evidenz ausreichend
- Accessibility-kompatibel
- AI-anwendbar + validierbar
- Anti-Pattern vorhanden
- Konflikte explizit dokumentiert

### WP6 — Atomic Skills (erst danach)

Skills aus CORE Rules; ein Skill = eine Aufgabe. Universal Skills = Source of Truth.

---

## Sprint-Schnitt Wave A (empfohlen)

| Sprint | Fokusquellen | Output |
| --- | --- | --- |
| S1 | WCAG 2.2, APG, NN/g Heuristics | A11y + Usability principle seeds |
| S2 | Carbon, Polaris, Primer (Foundations pages) | Color / Type / Spacing consensus candidates |
| S3 | Material 3 + Apple HIG (Foundations / Layout) | Platform-context splits |
| S4 | Forms + Buttons across Polaris/Carbon/Atlassian | Component principle candidates |
| S5 | 3–5 high-quality conference/system videos | Speech vs visual method rehearsal |
| S6 | Cross-source synthesis Wave A | Contradiction log + CORE candidates |

Instagram/Reels: frühestens nach S5 als **Noise-filtered** Batch, nie als alleinige CORE-Evidence.

---

## Methodenregeln (verbindlich)

1. Eine Designer-Aussage ≠ Regel.
2. Confidence steigt nur mit Evidence Mix (`06-standards-evidence.md`).
3. Bei Konflikt: P0–P7 Hierarchie; keine Fake-Consensus.
4. Keine exakten Token-Werte ohne belastbare Quelle; lieber Prinzip beschreiben.
5. Jede Normalisierung muss Originalaussage referenzieren.
6. Bestehende Rules dürfen sich durch neue Evidenz ändern — Changelog führen.

---

## Repo-Layout (Ziel)

```text
docs/intelligence/
├── README.md
├── research/                 ← Phase 0 (jetzt)
├── schemas/
├── sources/                  ← Phase 1
├── analysis/                 ← Phase 2
├── principles/               ← Phase 3
├── synthesis/                ← Phase 4
├── rules/                    ← Phase 5
├── evidence/
├── anti-patterns/
└── skills/                   ← Phase 6+
    └── universal/
```

---

## Definition of Done — Phase 0

- [x] Wichtigste Themen priorisiert
- [x] Experten/Creator tiered
- [x] Instagram/Video-Quellenstrategie definiert (ohne voreilige Skill-Ableitung)
- [x] Design-Systeme als Study Targets gelistet
- [x] UX/A11y-Standards als Evidenzanker gesetzt
- [x] Empirische Evidenzquellen benannt
- [x] Research-Plan mit Work Packages & Sprint-Schnitt

## Definition of Done — Phase 1

- [x] Source Profiles für `ST-001`, `ST-002`, `ST-003`, `DS-002`, `DS-003`, `DS-005`
- [x] Capture-Checklists Docs vs Video
- [x] Contradiction-Log Stub
- [x] Index + Status für weiteres Seed-Set
- [x] Keine Skill-Generierung

## Nächste konkrete Aktion (Phase 2 continue)

1. Frame-capture for VID-SAMPLE-001 demo UI (optional upgrade from partial)
2. Carbon/Polaris/Primer Foundations pages → claim inventories
3. APG Dialog + Tabs → Principle cards
4. Cross-check PRINCIPLE-RADIUS-001 against DS radius docs → keep EXPERIMENTAL or lift to CANDIDATE

**Skills werden erst nach Wave-A Canonical Rules erzeugt.**
