# Learning Notes — Bad Volume Controller

## Project goal

Build a tiny web page that lets a person make sound quieter or louder by choosing a point in a set of ripple rings. The interesting part is not advanced programming; it is observing how a person figures out an unfamiliar interface.

For the first version, use five clickable circles instead of real water animation, dragging, audio files, or an app framework. Each circle represents a volume level.

## What to learn, in order

### 1. Make a page

Learn the three basic web files:

- **HTML** gives the page its parts: title, hint text, and five buttons/circles.
- **CSS** makes those parts look like ripple rings.
- **JavaScript** makes the circles respond when someone clicks them.

Start with one `code/index.html` file, even if it contains a little CSS and JavaScript. Keeping everything together makes the first experiment easier to understand.

### 2. Store one piece of information

The interface needs to remember its current volume. In JavaScript, that can be one variable:

```js
let volumeLevel = 3;
```

Think of a variable as a labeled box that holds a value. Here, `3` could mean the middle ring out of five.

### 3. Respond to a click

Each ring needs an event listener: code that waits for a user action.

```js
ring.addEventListener("click", () => {
  volumeLevel = 4;
});
```

This teaches a foundational idea: programs can wait, then react to an event.

### 4. Update what the learner sees

After changing the value, update a message and highlight the selected ring:

```js
message.textContent = "The ripples are reaching farther.";
```

This is the important learning-design loop:

`action → program changes state → interface gives feedback → person forms an explanation`

### 5. Add real volume only after the interaction works

Browsers provide an `Audio` object whose `.volume` property uses a value from `0` (silent) to `1` (full volume). A five-level interface could convert its ring number like this:

```js
audio.volume = volumeLevel / 5;
```

Do this last. It requires a short audio file and browser permission to begin playing sound, so it can distract from the main interaction lesson.

## Small build plan

1. Create `code/index.html` with a heading, one hint, and five ordinary buttons.
2. Make each button set a different `volumeLevel`.
3. Display the selected level as text, such as “Ripple 2 of 5.”
4. Style the buttons as concentric circles with CSS.
5. Replace the level text with the learning-oriented hints from `Design.md`.
6. Ask one person to try it without instructions; note what they try and what they say they think it means.

Stop at any step and test it in a browser. A working small step is more useful than a large unfinished feature.

## What to observe in a user test

- What do they try first: center, outer ring, or random clicking?
- Can they explain which direction makes sound louder after one or two attempts?
- Which visual or text hint helps them form that explanation?
- Where do they hesitate or make an incorrect prediction?

Write observations, not judgments. For example: “They tapped the outer ring first, then said it looked like a target.” This can guide the next design change.

## Vocabulary to keep nearby

| Term | Plain-language meaning |
| --- | --- |
| HTML | The structure and content of a web page |
| CSS | The visual appearance of a web page |
| JavaScript | Instructions that make a web page react and change |
| Variable | A named place to store a value |
| Event | Something that happens, such as a click |
| State | The current information the program remembers, such as the selected volume level |
| Feedback | The visible or audible result after an action |

## Scope guardrail

This project does **not** need accounts, a database, a server, a mobile app, an animation library, or a complex sound system. If a feature makes the learning question harder to test, leave it for later.
