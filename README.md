# HIDE

A top-down stealth game. One finger. Twenty rooms. Don't be seen — and don't be heard.

**Play:** https://tonbonami.github.io/hide/

## The idea

Most stealth games punish you for being *seen*. This one also punishes you for being *fast*.

- **Speed = noise.** Move quickly and a sound ring spreads out. Guards nearby turn and come looking.
- **Vision cones are blocked by walls.** Real line-of-sight raycasting — step behind a crate and you vanish.
- **Shadows hide you** if you hold still. They also break an active chase.
- **The crowd hides you** — stand among the wandering civilians and you're much harder to pick out.
- **Gems sit on the guards' patrol routes.** Optional. And you lose them if you're caught.

Every second is the same question: *rush, or creep?*

## Technical

- Single HTML file, **~30 KB**
- **Zero external resources** — no CDN, no fonts, no images, no analytics. Sound is synthesized with WebAudio.
- Canvas2D, 60 FPS, 16:9 responsive (960×540 design space, letterboxed)
- Works in incognito (localStorage failures are caught)
- Touch and keyboard (WASD / arrows, hold Shift to sneak)

## Controls

- **Touch / mouse:** hold and drag. The further your finger is from the character, the faster they move — and the more noise they make.
- **Keyboard:** WASD or arrow keys. Hold **Shift** to sneak.

## Levels

20 levels, procedurally generated from a fixed seed — level N is always the same level. Guards, sight range, and map density scale up; crowd and shadows thin out.

Licensed to the author. All code original.
