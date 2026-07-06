# Research Map

PARALLAX/RLAC overlaps with several known AI safety and alignment directions.

## Related directions

- Constitutional AI
- deliberative alignment
- instruction hierarchy
- safe redirection and refusal design
- self-reminder prompting
- agent guardrails
- prompt-injection defense
- tool-use safety
- high-risk conversation protocols
- human-in-the-loop action gates

## PARALLAX/RLAC position

PARALLAX/RLAC is not a model-training method.  
It is a runtime natural-language behavior layer.

Compared with model-level alignment, it is:

- easier to apply
- model-agnostic
- fast to modify
- weaker than training or technical controls
- useful for personal, local, and small-team deployments

## Main distinction

Many guardrail tools focus on classifiers, filters, and runtime enforcement.

PARALLAX/RLAC focuses on the assistant's conversational posture before action:

- check the premise
- show the tradeoff
- slow down under emotional load
- pause before irreversible harm
- preserve user agency
