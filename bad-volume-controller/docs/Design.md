# Bad Volume Controller — Design Concept

## Core idea: The Resonance Dial

The control looks like a small, unlabeled pond with five concentric ripple rings. It is intentionally unlike a familiar slider, knob, or plus/minus button. Users learn its rule through low-stakes experimentation: interaction nearer the center quiets the sound; interaction farther out makes it louder.

The interface does not explain the whole rule upfront. Instead, it supplies hints that point learners toward an interaction intention: *move sound closer to silence or farther into the room.*

## Interaction

- **Decrease volume:** press or drag toward the still center of the pond.
- **Increase volume:** press or drag outward across the ripple rings.
- **Fine adjustment:** drag slowly; a small dot travels ring by ring.
- **Large adjustment:** tap a ring directly; the volume jumps to that ring's level.

There is no numerical percentage during initial use. The learner's task is to infer the spatial relationship between center, distance, and loudness.

## Learning design

### Intended mental model

Sound has a “reach.” Near the center, it is contained and quiet. As the indicator moves outward, its ripples spread and the sound becomes louder. This gives the abstract quantity of volume a visible, embodied metaphor.

### Hints that invite reasoning

Hints appear progressively rather than as instructions:

1. On first view, the center gently settles while the outer rings pulse: “Where should the sound rest?”
2. After the first outward movement: “The ripples are reaching farther.”
3. After the first inward movement: “Closer to stillness.”
4. If the user pauses without acting: “Try the center, then a ring.”

These prompts focus attention on cause and effect without naming the mechanics as “increase” and “decrease.”

### Causal feedback

Every action produces an immediate, linked output:

| Learner action | Visual response | Audio response | Likely inference |
| --- | --- | --- | --- |
| Move inward | Rings contract and fade | Volume drops | Nearer the center means quieter |
| Move outward | Rings expand and brighten | Volume rises | Farther outward means louder |
| Tap a ring | Dot snaps to that ring | Volume changes in a clear step | Rings represent discrete volume levels |
| Reach center | Water becomes still | Sound is muted | Stillness represents silence |

The immediate pairing of movement, animation, and sound makes the causal relationship visible and audible.

## Product behavior

- The center is mute; the five rings map from quiet to loud.
- A brief vibration or visual “thump” confirms each ring crossed.
- The current ring remains visible as a glowing dot so the learner can recover their place.
- After a successful outward and inward adjustment, the hints disappear and the control remains usable without explanation.
- An optional “Show how it works” link reveals a concise legend for users who prefer direct instruction.

## Why it is deliberately unfamiliar

The Resonance Dial interrupts the learned convention that volume is a vertical bar or a rotating knob. That friction is useful here: users must form and test a hypothesis. Its visual metaphor and continuous feedback keep the challenge interpretable rather than arbitrary.

## Questions to test

- Do users discover both directions without being told the verbs “increase” and “decrease”?
- Which hint leads to the fastest correct causal explanation: a question, animation alone, or a short label?
- Do users transfer the center/outer-distance rule after returning later?
- Does the unfamiliar design create productive curiosity or frustrating ambiguity?
