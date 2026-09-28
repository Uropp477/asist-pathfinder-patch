# mineflayer-pathfinder 2.4.5 — community patch

A drop-in patch for [mineflayer-pathfinder](https://github.com/PrismarineJS/mineflayer-pathfinder) 2.4.5,
tested in the `asist` autonomous Minecraft bot (Paper 1.21.11, mineflayer 4.x).

Fixes:

- **Leaves (`*_leaves`) are cheap to break** — the bot cuts through forests instead of
  standing still or taking huge detours (related:
  [#222](https://github.com/PrismarineJS/mineflayer-pathfinder/issues/222)).
- **Open doors** — corrected arrival point at doors (no more blocking on the door wing).
- **Trapdoors** — opened instead of broken; open trapdoors are passable.
- **Vines** (`vine`, `weeping_vines`, `twisting_vines`, `cave_vines` + `_plant`) — climbable.
- **Arrival threshold 0.35 → 0.175** — less jitter and fewer stuck-on-edge cases.
- **Lava** — the bot escapes lava instead of avoiding it while standing in it.

Parts of the patch are adapted from
[mindcraft-bots/mindcraft](https://github.com/mindcraft-bots/mindcraft) (MIT).

## Requirements

- `mineflayer-pathfinder` 2.4.5
- `mineflayer` 4.x
- Node.js 20+

## Install

```bash
npm install patch-package --save-dev
