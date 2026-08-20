## Agent skills

### Issue tracker

Issues and specs live as GitHub issues in this repo via the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default triage vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix` (plus category labels `bug` / `enhancement`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context layout: one `CONTEXT.md` at the repo root plus `docs/adr/`. See `docs/agents/domain.md`.

### Design System Intelligence

Research lives under `docs/intelligence/`. Wave A (Phases 0–8) and Wave B are complete: 11 CORE rules, 11 universal skills, model adapters, validation (`wave-a-core` + `wave-b-core`). Start at `docs/intelligence/README.md`. Prefer CORE over CANDIDATE.
