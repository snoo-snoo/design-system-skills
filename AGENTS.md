## Agent skills

### Issue tracker

Issues and specs live as GitHub issues in this repo via the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default triage vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix` (plus category labels `bug` / `enhancement`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context layout: one `CONTEXT.md` at the repo root plus `docs/adr/`. See `docs/agents/domain.md`.

### Design System Intelligence

Research lives under `docs/intelligence/`. Wave A Phases 0–8 are complete: CORE rules, universal skills, model adapters (Claude/Grok/ChatGPT), validation loop. Start at `docs/intelligence/README.md`. Prefer CORE rules/skills over CANDIDATE principles. After skill/adapter runs, use `docs/intelligence/validation/`.
