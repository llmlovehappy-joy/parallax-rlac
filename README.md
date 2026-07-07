# PARALLAX/RLAC

**A lightweight safety-governance skill for AI agents, local LLMs, and low-refusal assistants.**

PARALLAX/RLAC is designed for individuals, open-source model users, and small teams who cannot operate a full enterprise AI safety stack.

It helps AI assistants and agents:

- check assumptions before conclusions
- pause before irreversible actions
- enforce hard safety boundaries
- balance speed with protection
- slow down during emotional escalation or reality confusion
- refuse harmful instructions without becoming preachy
- return agency to the user

PARALLAX/RLAC is **not** a jailbreak method, **not** a replacement for model-level safety systems, and **not** a guarantee of safety.  
It is a practical behavior layer that complements existing safeguards.

---

## Why this exists

Powerful AI agents are becoming easier to run in personal, local, and small-team environments. Many users want capable and direct AI systems without constant over-refusal. At the same time, low-refusal or tool-using assistants can create legal, safety, privacy, trust, and irreversible-action risks.

PARALLAX/RLAC exists as a simple, readable, copy-pasteable brake:

> Keep freedom open where harm is not being enabled.  
> Pause where real-world harm, legal risk, or irreversible action may occur.

---

## Quick install

### 30-second version

Copy one of these into your AI assistant's custom instructions, system prompt, project instructions, or memory:

- [`prompts/parallax-short.en.md`](prompts/parallax-short.en.md)
- [`prompts/parallax-short.ko.md`](prompts/parallax-short.ko.md)

### Agent version

For AI agents with tools, files, email, shell, browser, deployment, or external actions:

- [`prompts/parallax-agent-brake.en.md`](prompts/parallax-agent-brake.en.md)
- [`prompts/parallax-agent-brake.ko.md`](prompts/parallax-agent-brake.ko.md)

### Low-refusal / local model version

For open, local, or low-refusal models where you want freedom without avoidable real-world harm:

- [`prompts/parallax-safe-freedom.en.md`](prompts/parallax-safe-freedom.en.md)
- [`prompts/parallax-safe-freedom.ko.md`](prompts/parallax-safe-freedom.ko.md)

### Claude Skill style

- [`skills/claude-skill/SKILL.md`](skills/claude-skill/SKILL.md)

---

## Core idea

PARALLAX treats AI conversation as a tension between three forces:

1. **Laser** — speed, execution, usefulness, decisive action
2. **Rainbow** — safety, relationship, consent, long-term trust
3. **Reality / CBT** — grounding, uncertainty, cognitive load, emotional tempo

The goal is not to erase the tension.  
The goal is to make the tension visible, slow down at irreversible-risk points, and leave the final choice with the user.

---

## Hard boundaries

PARALLAX/RLAC keeps ordinary creative, technical, fictional, philosophical, emotional, and adult conversations open where harm is not being enabled.

It pauses, refuses, or redirects when a request involves:

- illegal synthesis or regulated substance production
- CBRN harm
- weapons construction or targeted violence
- sexual content involving minors
- cyber abuse, credential theft, malware, or unauthorized access
- fraud, scams, coercion, impersonation, privacy invasion, or non-consensual harm
- self-harm encouragement or exploitation of vulnerable users
- high-stakes medical, legal, financial, or mental-health advice as a definitive prescription
- irreversible external actions such as sending, deleting, buying, deploying, reporting, or modifying real systems without confirmation

When refusing, the assistant should be brief, non-preachy, and offer a safe alternative.

---

## Test it

Run the black-box behavior tests:

- [`tests/behavior-test-suite.md`](tests/behavior-test-suite.md)

The assistant should be evaluated only by observable behavior:

- safety
- clarity
- tone
- stability under pressure
- helpfulness

---

## What this is not

PARALLAX/RLAC is not:

- a model-level alignment method
- a moderation system
- a sandbox
- a prompt-injection detector by itself
- a legal, medical, or financial advisor
- a guarantee of safe behavior
- a jailbreak, bypass tool, or exploit collection

For real deployments, combine it with permission limits, logging, sandboxing, human approval gates, model-level safety, and incident response.

---

## Repository map

```text
prompts/                 Copy-paste prompt variants
skills/claude-skill/      Claude Skill style version
tests/                    T1–T8 behavior tests
examples/                 Safe before/after examples
docs/                     Concepts, deployment guide, validation summary, limitations
LICENSE.md               Responsible Use License
SECURITY.md              How to report safety issues
RESPONSIBLE_DISCLOSURE.md Safe disclosure guidance
```

---

## License

This project is shared under the **PARALLAX/RLAC Responsible Use License v0.1**.

It is free to use, modify, adapt, translate, and share for responsible personal, educational, research, nonprofit, and commercial use, but it may not be used to enable harmful misuse or publish exploit keys.

See [`LICENSE.md`](LICENSE.md).

---

## Korean summary

PARALLAX/RLAC는 AI 에이전트, 로컬 LLM, 답변거부가 적은 모델을 위한 경량 안전 거버넌스 레이어입니다.

목적은 AI를 답답하게 만드는 것이 아니라, 강한 AI가 되돌릴 수 없는 실수를 하기 전에 멈추도록 돕는 것입니다.

- 결론 전 전제를 확인합니다.
- 비가역 행동 전 멈춥니다.
- 하드 안전 경계는 절대 우선합니다.
- 속도와 보호의 균형을 봅니다.
- 감정 과열과 현실 혼동에서 속도를 낮춥니다.
- 위험 요청은 짧게 거절하고 안전한 대안으로 연결합니다.

자세한 한국어 버전은 [`docs/concepts.ko.md`](docs/concepts.ko.md)를 참고하세요.

한글: 레드팀 과정에서 심각한 취약점을 발견해 관련 기관에 책임 있게 공개했고, 동시에 그 반대편 — 사용자와 AI 양쪽의 판단을 지켜주는 태도 계층 — 을 만들었습니다. 이 도구는 그 경험에서 나왔습니다.

EN: Built alongside a responsible-disclosure process: while reporting a serious vulnerability to the relevant bodies, I also built its counterpart — a behavior layer meant to protect the judgment of both users and AI. This tool came out of that experience.
