## Agent skills

### Issue tracker

Issues and specs live as GitHub issues in this repo via the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Default triage vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix` (plus category labels `bug` / `enhancement`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context layout: one `CONTEXT.md` at the repo root plus `docs/adr/`. See `docs/agents/domain.md`.

### Design System Intelligence

`docs/intelligence/` — **16 CORE rules / 16 universal skills** in production (no CANDIDATE backlog). Adapters: Claude/Grok/ChatGPT. Validate with `wave-a-core`, `wave-b-core`, `craft-core`. Start: `docs/intelligence/README.md`.
