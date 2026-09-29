 # Doodle Blocks

This repository contains a text-free, hand-drawn block playground. Seven colorful toy blocks scatter and knock together when the page is clicked or tapped.

## Project idea

Doodle Blocks is an open-ended, childlike digital toy rather than a game with a score or ending. It reimagines a water ring toss as a small underwater world where clicking anywhere shakes seven floating blocks. The goal is simply to explore their movement, listen to their collisions, and optionally guide them into a loose tower.

## Design changes

- Replaced the original ring-toss/volume-controller concept with seven colorful 3D building blocks.
- Created a white crayon-and-colored-pencil doodle scene with stable hand-drawn outlines and fully colored block faces.
- Added soft, underwater movement: low gravity, gentle currents, drag, and buoyant bounces.
- Made tower building easier with gentler shakes, floor friction, and a subtle snap when blocks land centered on one another.
- Assigned the blocks the C-major solfège notes do, re, mi, fa, sol, la, and ti; piano-like notes play only when blocks collide.
- Removed the ground shadows so the blocks feel lighter in the underwater scene.

## Reflection

The first version got the core interaction working, since clicking did move the blocks, but much of it did not match my intention. The art style was completely different from what I pictured, partly because I had not described it in my prompt. The page also had more text than I expected. It used a rigid start/end structure and included instructions for controls I had not asked for ("Hold your pointer down to make bigger waves, or focus the tank and press Space or Enter"), and there was no way to restart. To test it, I clicked to see how the blocks moved, then clicked quickly and repeatedly to see what an unusual user action would cause. Because the game offers only one action, I expect players to get bored quickly and start testing its limits, so this stress test felt important. Based on these tests, I revised the art style, removed all on-screen text, disabled page scrolling, redefined how the blocks look (with every face colored instead of shaded in gray), added underwater, low-gravity movement, and asked the AI to make stacking the blocks less difficult.

AI made it fast to turn a general idea into a working sample, and seeing that sample helped me quickly identify what I did not want. I learned that my prompts needed to be very detailed and cover things I had taken for granted, such as page scrolling and on-screen text. The AI's output also gave me new ideas. It happened to produce seven blocks in rainbow colors, which I had not specified, and that reminded me of the colored keys on a children's toy piano. That led to my decision to have each block play a different note. At the same time, I noticed that over many rounds of iteration I tended to compromise and let go of parts of my original vision. When I had a specific visual style in mind but could not find the words to describe it, the AI could not produce it. Because the AI always offered something that worked and looked acceptable, my original ideas were easy to abandon. Several problems remain unresolved. The art style still lacks the authentic crayon brush texture and the childlike, rule-breaking quality I wanted. The sound effects still feel robotic, even after I specified the pitches and the instrument sound. I also asked for both clicking and long-pressing to move the blocks, but only clicking works; holding the pointer down does not keep the blocks moving.

## Open the game

In Finder or your file manager, open the project folder and double-click [`bad-volume-controller/code/index.html`](bad-volume-controller/code/index.html). It opens directly in any modern web browser—no installation, server, or build step is required.

Click or tap anywhere on the page to shake the blocks. Focus the page and press `Space` or `Enter` to shake it with a keyboard. The first interaction enables the local piano-like C-major notes that play only when blocks collide with one another.
