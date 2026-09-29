# Bad Volume Controller — Working Policy

## Purpose

This is a beginner-friendly learning-sciences prototype. Its purpose is to explore how people learn an unfamiliar interface, not to build a feature-complete audio product.

## Implementation policy

- Prefer the smallest working implementation that can test one interaction idea.
- Use plain HTML, CSS, and JavaScript before adding libraries, frameworks, build tools, servers, accounts, databases, or external services.
- Introduce one computational concept at a time and explain it in plain language in `docs/learning-note.md`.
- Keep the runnable prototype in `code/` and design/learning documentation in `docs/`.
- Keep `README.md` blank unless the project owner explicitly asks to change it.
- Avoid adding features that do not help answer the learning question.

## Interaction-design policy

- Preserve the intentionally unfamiliar “resonance dial” metaphor: center means stillness/mute; moving outward means louder sound.
- Let people infer the rule through action and immediate causal feedback before supplying direct instruction.
- Use progressive hints that describe consequences (for example, “The ripples are reaching farther”) rather than conventional control labels whenever practical.
- Make current state visible through the interface, such as the orange indicator dot and clear status text.
- Make the control forgiving: a user should not need pixel-perfect clicks to achieve an intended action. The innermost circle is a mute zone.
- Keep a keyboard-accessible path, even when the main interaction is experimental or unfamiliar.

## Evaluation policy

- Treat confusion as evidence, not as user failure.
- When testing, record what people do, predict, say, and hesitate over before deciding on a change.
- Test a change in the browser after making it when possible.
- If an observation reveals a mismatch between the intended rule and actual use, simplify or clarify the interface before adding complexity.

## Change checklist

Before implementing a feature, ask:

1. Does it help people discover or understand the cause-and-effect rule?
2. Can it be made with concepts appropriate for a beginner programmer?
3. Does it belong in `code/` or `docs/`?
4. Can the result be tested with one person in a short session?
