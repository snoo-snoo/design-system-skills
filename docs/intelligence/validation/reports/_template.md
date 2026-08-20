# Validation Report Template

Copy to `reports/YYYYMMDD-<target-slug>.md` (or emit inline in model output).

```text
REPORT-ID: VR-YYYYMMDD-##
Target:
SkillsApplied:
RulesInScope:
ModelAdapter: claude | grok | chatgpt | none
Timestamp:

CHECKS:
| Checklist | Item ID | Result | Severity | Evidence | Remediation |
| --- | --- | --- | --- | --- | --- |
| wave-a-core | WA-01 | pass/fail/n/a/needs-info | P0 |  |  |

SUMMARY:
  PassCount:
  FailCount:
  Blockers:
  Verdict: pass | pass-with-warnings | fail

ASSUMPTIONS / NEEDS-INFO:
  -

FEEDBACK_TO_RULES: (optional — route to research)
  -
```

Schema: [`../../schemas/validation-report.md`](../../schemas/validation-report.md)
