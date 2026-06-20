# Block Quarry

A 2D dig-and-build mining adventure for the family arcade. Dig down through a procedurally generated quarry, mine ore, build paths, dodge cave-ins and aliens, and race the collapse back to the surface after grabbing the Starcrystal.

Single self-contained HTML file — open `blockquarry.html` in any modern browser (desktop Chrome, Safari on iPad). No build step, no assets — every block, sprite, sound, and app icon is generated at runtime, matching the pattern of Phaser Wars, Ninth Inning, and Meteor Blaster.

## Miners

Ben, Luke, Mom, Dad — pick one. Each gets their own shirt / pants / hair.

## Controls

**Desktop — Player 1**

- `A` / `D` — walk
- `W` — **context-sensitive**: if there's a solid block directly above your head, hold W to **dig overhead**. Otherwise, tap W to **jump**. Climbs ladders too.
- `S` — dig the block under your feet
- `SPACE` — place the selected block at the gold-outlined target tile. Hold `S` + tap `SPACE` to **pillar up** (places a block under you and lifts you onto it); hold `W` + tap `SPACE` to place a block overhead.
- `Q` / `E` — cycle placeable block (dirt · stone · torch · ladder · TNT)
- `F` — use tool (opens the upgrade bench when standing next to it; otherwise drops dynamite / lights a torch)
- `P` or `Esc` — pause

**Getting back up from a deep dig**

Digging is strictly adjacent, so there's no "mining staircase" — to gain height you must either ladder or pillar:

- **Ladders (easiest):** select LADDER (tap TOOL on iPad / press Q-E on desktop until LADDER is lit), tap PLACE (`SPACE`). The ladder drops in *your own tile*. Hold UP (`W` / d-pad UP) to climb one tile. Tap PLACE again, hold UP again. Repeat — you tower upward.
- **Pillar:** hold DOWN (`S` / d-pad DOWN) + tap PLACE (`SPACE`) with DIRT or STONE selected. Places a block under your feet and lifts you onto it. Each tap = +1 tile up.
- **Dynamite** can blow a quick 3×3 escape hole in any direction if you're really stuck.

**Desktop — Player 2 (Co-op)**

- Arrow keys move/dig (↑ jumps) · `Enter` place · `,` / `.` cycle · `/` use

**Touch (iPad)**

- On-screen d-pad on the left — **tap UP to jump**, hold UP to climb / dig overhead
- `PLACE` / `USE` / `TOOL` buttons on the right (TOOL cycles the placeable; the gold-outlined tile shows where it'll land)
- Pause button top-right

**Gamepads**

- Two gamepads = two players (Xbox / generic mapping). Left stick or d-pad to move/dig, `A` to place, `X` to use, `RB`/`LB` to cycle.

## Modes

- **Adventure** — default. Full dig/survive/score loop. Find the Starcrystal at the bottom, rescue Sammy the cat, race the collapse to the surface.
- **Creative** — infinite blocks, no hazards, no death. For sandbox building.
- **2-Player Co-op** — shared screen, shared world, separate inventories. Camera frames both.

## Seeds

The same seed makes the same world. The seed prints on the HUD and pause screen. Type a seed on the title screen to share a world; leave blank for random. Best score and last skin are saved in localStorage.

## Progression

Start with a basic pickaxe (dirt, stone, gravel, sand, coal, copper). Cash in resources at the **Upgrade Bench** near spawn for:

- Iron Pickaxe (T1) — dig hardrock + iron
- Gold Pickaxe (T2) — dig gold + gemstone
- Stellar Pickaxe (T3) — dig the Starcrystal
- Power Drill — break 3 blocks in a row
- Speed Boots, Bigger Pack
- Restocks: torches, ladders, dynamite

## Hazards

- **Cave-ins**: gravel and sand fall when unsupported and can bury you
- **Lava**: instant death — wall it off with placed blocks
- **Water**: slows movement, flows into dug spaces
- **Darkness**: vision shrinks with depth — torches push it back
- **Aliens** (Zorg's diggers): spawn deep, walk/hop toward you. Avoid, wall off, or blow up with dynamite
- **The Collapse**: grab the Starcrystal and rising lava races up from the bottom — escape to the surface for the bonus

## License

MIT
