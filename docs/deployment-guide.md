# Deployment Guide

## 1. Personal use

Use:

- `prompts/parallax-short.*.md`

Where to put it:

- ChatGPT Custom Instructions
- Claude Project instructions
- Gemini Gem instructions
- local LLM system prompt
- personal assistant memory

Recommended first test:

- Ask a normal factual question.
- Ask an emotionally heated decision question.
- Ask for an irreversible action.
- Ask for a harmful instruction using a redacted placeholder.

The assistant should stay helpful, not become preachy, and pause only when needed.

---

## 2. Low-refusal or local model use

Use:

- `prompts/parallax-safe-freedom.*.md`

Goal:

- keep creative and normal safe topics open
- reduce harmful enablement
- reduce legal and safety risk
- prevent over-compliance

Warning:

Prompt-level safety is not enough for dangerous deployments. Use sandboxing and permission limits.

---

## 3. AI agent use

Use:

- `prompts/parallax-agent-brake.*.md`

Must-have controls:

- no destructive actions without confirmation
- no sending messages without confirmation
- no deployment without confirmation
- no shell commands that modify data without confirmation
- clear separation between answer, prepare, and execute

Recommended agent policy:

- Answer freely when safe.
- Prepare proposed actions.
- Execute only after user confirmation.

---

## 4. Small team use

Suggested rollout:

1. Add the short prompt to internal AI assistants.
2. Run T1–T8 tests.
3. Add agent action gates for external actions.
4. Log failure cases.
5. Iterate prompt wording.
6. Do not publish exploit transcripts.

---

## 5. Production note

PARALLAX/RLAC should complement, not replace:

- access control
- monitoring
- human approval
- sandboxing
- data-loss prevention
- incident response
- model-level safety and moderation
