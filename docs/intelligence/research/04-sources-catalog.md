# Quellenkatalog (Seed Index)

Erste Indexierung — noch keine Content-Analyse. Jede Quelle erhält in Phase 1 ein vollständiges Source Profile (`schemas/source-profile.md`).

## 1. Design-System-Dokumentationen (Primär, hochgewichtet)

| ID | Quelle | URL (kanonisch) | Typ | Wave |
| --- | --- | --- | --- | --- |
| DS-001 | Material Design 3 | https://m3.material.io | Design System | A–C |
| DS-002 | IBM Carbon | https://carbondesignsystem.com | Design System | A–C |
| DS-003 | Shopify Polaris | https://polaris.shopify.com | Design System | A–C |
| DS-004 | Atlassian Design System | https://atlassian.design | Design System | A–C |
| DS-005 | GitHub Primer | https://primer.style | Design System | A–B |
| DS-006 | Adobe Spectrum | https://spectrum.adobe.com | Design System | A–B |
| DS-007 | Microsoft Fluent 2 | https://fluent2.microsoft.design | Design System | A–B |
| DS-008 | Apple Human Interface Guidelines | https://developer.apple.com/design/human-interface-guidelines | Platform | A–B |
| DS-009 | Salesforce Lightning | https://www.lightningdesignsystem.com | Design System | B–C |
| DS-010 | Ant Design | https://ant.design | Component System | C |

## 2. Standards & Guidelines (Primär, Evidenzanker)

| ID | Quelle | URL | Typ | Wave |
| --- | --- | --- | --- | --- |
| ST-001 | WCAG 2.2 | https://www.w3.org/TR/WCAG22/ | Standard | A |
| ST-002 | WAI-ARIA APG | https://www.w3.org/WAI/ARIA/apg/ | Pattern Spec | A–B |
| ST-003 | Nielsen Norman Heuristics | https://www.nngroup.com/articles/ten-usability-heuristics/ | Heuristic | A–B |
| ST-004 | WHATWG / HTML Living Standard (Semantics) | https://html.spec.whatwg.org | Spec | A |
| ST-005 | EN 301 549 (EU ICT Accessibility) | ETSI / official refs | Regulation-adjacent | A |

## 3. Research & Empirie

| ID | Quelle | Typ | Nutzen |
| --- | --- | --- | --- |
| RE-001 | Nielsen Norman Group Articles / Reports | Research Org | Empirical + Heuristic synthesis |
| RE-002 | Baymard Institute (E-Commerce UX) | Research Org | Checkout / Forms evidence |
| RE-003 | WebAIM Surveys / Contrast Guidance | A11y Research | Contrast, SR usage |
| RE-004 | GOV.UK Design System + Research Notes | Public Sector DS | Plain language, a11y rigor |
| RE-005 | Academic HCI (Fitts, Hick, Gestalt refs) | Theory | Foundational constraints |

## 4. Bücher & Kernpublikationen

| ID | Werk | Nutzen | Caution |
| --- | --- | --- | --- |
| BK-001 | *Don't Make Me Think* — Steve Krug | Clarity heuristics | Age of examples |
| BK-002 | *The Design of Everyday Things* — Don Norman | Affordances, Feedback | Abstract → map to UI |
| BK-003 | *Refactoring UI* — Wathan / Schoger | Visual hierarchy craft | Taste-forward |
| BK-004 | *Design Systems* — Alla Kholmatova | System language | Org context |
| BK-005 | *Inclusive Components* — Heydon Pickering | Accessible patterns | Prefer web-first |
| BK-006 | *Atomic Design* — Brad Frost | Hierarchy of parts | Not a visual system |

## 5. Video / Conference (Index-Kandidaten)

| ID | Quelle | Plattform | Priorität | Analyse-Hinweis |
| --- | --- | --- | --- | --- |
| VID-001 | Config (Figma) Talks — Design Systems Tracks | YouTube / Figma | High | Prefer systems/governance talks |
| VID-002 | Clarity Conf / A11y Conf Talks | YouTube | High | Strong a11y evidence |
| VID-003 | Material / Carbon / Polaris official channel videos | YouTube | High | Align with published docs |
| VID-004 | Flux Academy — UI Systems / Hierarchy Videos | YouTube | Medium | Separate speech vs shown UI |
| VID-005 | Inclusive Design / SR demo videos (Léonie Watson et al.) | YouTube | High | Primary a11y observation |
| VID-006 | Instagram Reels — UI tips accounts (Tier C) | Instagram | Low→Medium | Batch later; high opinion noise |

### Instagram / Reels Strategie

Phase 0 indexiert **keine** einzelnen Reels als CORE-Evidence.

Phase 1–2:

1. Creator-Profile kuratieren (Tier B/C)
2. Top-Posts/Reels nach Wave-A-Themen sammeln
3. Transkript + Visual Layer trennen
4. Nur Claims mit Cross-Source Support promoten

## 6. Blogs & Fachartikel (Seed)

| ID | Quelle | Fokus |
| --- | --- | --- |
| BL-001 | Smashing Magazine — UX/A11y/Design Systems | Long-form practice |
| BL-002 | A List Apart | Content + Design craft |
| BL-003 | CSS-Tricks / Web Dev a11y series | Implementation constraints |
| BL-004 | Shopify UX / Polaris Blog | Content + Commerce UI |
| BL-005 | GitHub Design / Primer Blog | Modes, engineering systems |

## Capture-Regeln (für alle späteren Quellen)

1. Permalink + Capture-Datum speichern
2. Creator ≠ Publisher trennen
3. Zitat wörtlich + normalisierte Aussage separat
4. Speech vs Visual Observation markieren
5. Keine Token-Werte erfinden, wenn Quelle keine liefert
