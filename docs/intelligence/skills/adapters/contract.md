# Adapter Contract

Binding rules for all model adapters in this repo.

## Source of truth chain

```text
CORE Canonical Rule
        ↓
Universal Skill (must not be forked)
        ↓
Model Adapter (tone / shape only)
        ↓
Model output
        ↓
Validation Loop (Phase 8)
```

## Allowed adapter changes

- System/developer preamble style
- Verbosity defaults
- Preferred markdown/JSON framing
- Tool-calling hints (when the host supports tools)
- Reminder to run validation checklists

## Forbidden

- New MUST/SHOULD rules not present in the Universal Skill / CORE Rule
- Inventing spacing/color/radius token values
- Weakening P0 accessibility requirements for aesthetics
- Silently resolving open contradictions (CX-002, CX-004, …)
- Merging multiple Universal Skills into one “do everything” adapter

## Required footer on every adapter output request

Ask the model to finish with:

1. Self-review from the Universal Skill  
2. Validation Loop checklist results (`wave-a-core` at minimum)  
3. Explicit list of any assumptions / needs-info items  
