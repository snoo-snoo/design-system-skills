# Schema: Validation Report

Used by Phase 8 Validation Loop after skill/adapter output.

```text
REPORT-ID:
Target: (UI description / file / component)
SkillsApplied: [skill-ids]
RulesInScope: [RULE-ids]
ModelAdapter: claude | grok | chatgpt | none
Timestamp:

CHECKS:
  - Checklist: accessibility | consistency | ux | design-system | wave-a-core
    Item: ...
    Result: pass | fail | n/a | needs-info
    Evidence: ...
    Severity: P0..P7
    Remediation: ...

SUMMARY:
  PassCount:
  FailCount:
  Blockers: (any P0 fail)
  Verdict: pass | pass-with-warnings | fail

FEEDBACK_TO_RULES: (optional)
  - Observation that may update a Principle/Rule (route to research, not silent edit)
```
