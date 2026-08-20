# PRINCIPLE-FORM-FEEDBACK-001 — Immediate Form Interaction Feedback

```text
Principle:
Form interactions should provide timely visible feedback for focus, input,
validation, and progress without relying on motion alone.

Problem:
Silent forms increase uncertainty and error rates.

Recommendation:
Show clear focus/active states; validate with understandable messages; evolve
primary CTA with progress when helpful; honor `prefers-reduced-motion`.

Why:
Visibility of system status (NN/g #1); confidence in multi-step flows.

Context:
Multi-step and high-stakes forms (onboarding, payments).

Exceptions:
Offline/batch validation where immediate checks are impossible—communicate
pending state explicitly.

Evidence:
- VID-SAMPLE-004 (active states, CTA evolution, spatial continuity)
- ST-003 Heuristic #1
- PRINCIPLE-FOCUS-001

Confidence:
Medium–High

Category:
04 Patterns / Forms + 05 UX

StatementClass:
Practice + Heuristic

Maturity:
CANDIDATE

PriorityFloor:
P1 functional clarity / P0 when feedback is required for errors
```
