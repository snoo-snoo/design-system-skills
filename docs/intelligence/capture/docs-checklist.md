# Capture Checklist — Documentation Sources

Use for design-system docs, standards, research articles, and blog posts.

## Before capture

- [ ] Confirm canonical URL (prefer stable TR / docs root, not campaign pages)
- [ ] Record capture date (ISO-8601)
- [ ] Identify publisher vs individual author
- [ ] Note license / citation requirements if any
- [ ] Map primary taxonomy categories (01–09)

## What to capture

1. **Scope statement** — what the doc claims to cover
2. **Normative vs informative** — requirements vs guidance vs examples
3. **Foundations** — color, type, space, elevation, motion (as present)
4. **Components / patterns** — inventory of covered UI units
5. **States** — focus, disabled, error, loading, empty (explicit?)
6. **Accessibility** — dedicated guidance, WCAG mapping, keyboard
7. **Content** — labels, errors, tone, when-to-use
8. **Responsive / platform** — breakpoints, platform forks
9. **Token model** — primitive / semantic / component (if any)
10. **Governance signals** — versioning, deprecation, contribution

## Extraction discipline

- Quote or paraphrase with section anchor when possible
- Classify each claim: `Standard | System Convention | Heuristic | Practice | Opinion`
- Do **not** invent token numeric values
- Flag gaps explicitly (`not documented`)

## Output

- Update Source Profile status → `indexed` (profile complete) or `ready_for_analysis`
- Create analysis folder only in Phase 2: `docs/intelligence/analysis/<SOURCE-ID>/`
