# Model Adapters — Phase 7

Thin, model-specific wrappers around Universal Skills. **Universal Skills remain Source of Truth.**

| Model | Profile | Skill adapters |
| --- | --- | --- |
| Claude (Anthropic) | [claude/](claude/) | 7 wrappers |
| Grok (xAI) | [grok/](grok/) | 7 wrappers |
| ChatGPT (OpenAI) | [chatgpt/](chatgpt/) | 7 wrappers |

## Hard rules

1. Adapters **reference** Universal Skills — they do not restate or alter RULES.
2. Adapters may change tone, section order, tool hints, and output shaping only.
3. On conflict: CORE Rule → Universal Skill → Adapter (adapter loses).
4. After every adapter run, execute the [Validation Loop](../../validation/README.md).

## How to use

1. Pick model profile (`claude` / `grok` / `chatgpt`).
2. Open the matching skill adapter (same kebab name as Universal Skill).
3. Paste invoke block + attach Universal Skill path + user task.
4. Run Phase-8 validation on the output.

Schema: [`../../schemas/adapter.md`](../../schemas/adapter.md)  
Contract: [`contract.md`](contract.md)  
Shared invoke skeleton: [`invoke-template.md`](invoke-template.md)
