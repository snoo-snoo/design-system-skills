# Design-Systeme — Study Matrix

Studieren für **Entscheidungen und Architektur**, nicht für visuelle 1:1-Kopie.

## Primäre Study Targets

| System | Beste Lernsignale | Weniger kopieren |
| --- | --- | --- |
| **Shopify Polaris** | When-to-use / when-not; Content standards; Token intent | Commerce-spezifische Defaults |
| **IBM Carbon** | Per-component a11y; Governance; Open structure | Enterprise density as universal default |
| **Atlassian Design System** | Semantic tokens as stable API; Multi-product migration | Product-specific density |
| **GitHub Primer** | Color modes schema; Versioning as product | Developer-tool aesthetics |
| **Material 3** | Three-tier tokens; Theming / dynamic color model | Ecosystem lock-in visuals |
| **Apple HIG** | Platform conventions; Clarity of interaction roles | iOS-only patterns as web defaults |
| **Adobe Spectrum** | Evolving live systems; Token contracts | Creative-tool density |
| **Microsoft Fluent 2** | Cross-platform coherence | Platform-native exceptions ignored |
| **GOV.UK Design System** | Plain language; Accessibility rigor; Service patterns | Government formality as brand |
| **Ant Design** | Dense data UI patterns | Assuming density = good UX |

## Vergleichsachsen (für spätere Cross-Source Analysis)

Für jedes System und jedes Wave-A-Thema erfassen:

1. **Token model** — Primitive / Semantic / Component?
2. **State completeness** — Focus, Disabled, Error, Loading?
3. **Content guidance** — Labels, Errors, Empty?
4. **A11y docs depth** — Keyboard, SR, Contrast?
5. **Responsive strategy** — Breakpoints / adaptive / platform forks?
6. **Pattern coverage** — Forms, Tables, Nav, Feedback?
7. **Governance signal** — Versioning, deprecation, contribution?

## Ableitungsregel

Wenn ≥ 3 unabhängige Systeme dasselbe Prinzip dokumentieren **und** es nicht gegen WCAG/P0 verstößt → Kandidat für `CORE`.

Wenn Systeme widersprechen → Konflikt dokumentieren, Context splitten (z. B. Dense Enterprise Table vs Consumer Form), **keine künstliche Einigkeit**.
