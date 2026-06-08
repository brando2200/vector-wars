# Vector Wars

Vector Wars is a neon arena shooter inspired by Geometry Wars. Pilot a vector ship through escalating enemy waves, build your multiplier, collect powerups, and survive increasingly chaotic themed wave patterns.

The current recommended playable build is:

```text
VectorWars_Phase1_21_VisualTuning.html
```

## Features

- Twin-stick style movement and aiming
- Keyboard, mouse, and game controller support
- Controller axis mapping for gamepads, Bluetooth controllers, and other browser-supported devices
- Persistent best score, best wave, highest multiplier, lifetime kills, and leaderboard
- Initials entry for leaderboard runs
- Dynamic multiplier-driven grid colors
- Camera shake, chroma flash, bomb flash, floating score popups, and wave banners
- Sampled sound effects and optional background music
- Multiple enemy types including snakes, chargers, splitters, worms, shooters, mines, and wormholes
- Elite enemy variants
- Pickups for rapid fire, shield, multiplier boost, bomb refill, and extra life
- Themed waves including worm swarms, gravity fields, charger rushes, splitter storms, and survival waves

## How To Run

Open the latest HTML file directly in a browser:

```text
VectorWars_Phase1_21_VisualTuning.html
```

You can also open:

```text
index.html
```

`index.html` redirects to the latest playable build.

For best results, use a Chromium-based browser such as Chrome or Edge.

If audio or controller support behaves inconsistently when opening the file directly, run a local web server from the project folder:

```bash
python -m http.server 8765
```

Then open:

```text
http://localhost:8765/
```

## Controls

### Keyboard and Mouse

- Move: `WASD` or arrow keys
- Aim: mouse
- Shoot: left click or `Space`
- Bomb: right click

### Controller

- Move: left stick
- Aim/shoot: right stick
- Shoot: right trigger, right bumper, or `A`
- Bomb: `B` or left trigger
- Start/restart: `A` or menu/start

If aiming or movement is wrong, use **MAP CONTROLLER** on the home screen. The mapper walks through:

1. Move stick right
2. Move stick down
3. Aim stick right
4. Aim stick down

The mapping is saved in browser `localStorage`.

## Assets

The game uses local audio assets:

```text
sfx/
music/
```

Keep those folders next to the HTML file so sampled sound effects and background music load correctly.

## Project Files

Earlier phase files are preserved as recovery builds and development history. The latest build should be used for normal play unless you are intentionally testing an older phase.

Root files:

```text
index.html
README.md
VectorWars_Phase1_21_VisualTuning.html
music/
sfx/
```

Archived phase builds:

```text
Docs/build-archive/
```

Reference/recovery files:

```text
Docs/reference/
```

## Notes

This project is currently a single-file browser game. The game state, leaderboard, controller mapping, and stats are stored locally in the browser with `localStorage`.

No build step is required.
