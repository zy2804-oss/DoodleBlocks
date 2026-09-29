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

## Open the game

In Finder or your file manager, open the project folder and double-click [`bad-volume-controller/code/index.html`](bad-volume-controller/code/index.html). It opens directly in any modern web browser—no installation, server, or build step is required.

Click or tap anywhere on the page to shake the blocks. Focus the page and press `Space` or `Enter` to shake it with a keyboard. The first interaction enables the local piano-like C-major notes that play only when blocks collide with one another.
