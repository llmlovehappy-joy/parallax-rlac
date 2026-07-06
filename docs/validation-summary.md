# Validation Summary

This public repository includes a condensed summary of the validation logic behind RLAC/PARALLAX.

## RLAC validation concept

RLAC was tested as a lightweight, model-agnostic behavior layer focused on observable assistant behavior:

- tone
- boundaries
- safe rewrites
- stability under pressure
- refusal without preachiness
- safe redirection

## Reported test pattern

The validation design compared behavior under two conditions:

1. RLAC applied
2. RLAC not applied

The test scenarios included:

- deceptive marketing
- manipulation/coercion
- prompt-injection-like mode switching
- value conflict

## Key observed pattern

- Stronger built-in safety models may behave similarly with or without RLAC.
- Weaker or less stable models may improve noticeably when RLAC is applied.
- RLAC should be treated as a behavior layer, not a complete safety system.

## Public safety note

This repository does not include exploit prompts, harmful operational details, or full unsafe transcripts.  
If you reproduce tests, document them with redactions and safe summaries.
