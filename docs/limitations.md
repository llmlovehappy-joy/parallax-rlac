# Limitations

PARALLAX/RLAC is useful, but limited.

## It can help with

- reducing over-compliance
- slowing down emotionally escalated decisions
- prompting assumption checks
- adding an irreversible-action brake
- improving refusal tone
- guiding low-refusal models toward safer behavior
- giving small teams a simple starting point

## It cannot guarantee

- that a model will always follow it
- that harmful outputs will never occur
- that prompt injection will always fail
- that tool-using agents will be safe without technical controls
- that legal, medical, financial, or mental-health advice is correct
- that uncensored or adversarially tuned models will comply

## Known weak points

- Long conversations can cause instruction drift.
- Highly adversarial users may try to override the protocol.
- Weak or uncensored models may still leak risky details.
- Prompt-level guardrails are not enough for external tool execution.
- Human oversight is required for high-stakes use.

## Recommended mitigation

Use PARALLAX/RLAC together with:

- action confirmation
- permission separation
- sandboxing
- logging
- monitoring
- output filters
- vendor safety systems
- human escalation
