# VOIDRUN: Forbidden Sector

VOIDRUN is a small, static 3D arcade space combat game. Fight through three escalating fighter rounds, then destroy the Warden mothership to escape the sector.

## Run locally

No build step or package installation is needed. Three.js and the display fonts load from CDNs, so the game needs an internet connection.

Run a local web server from the project folder:

```sh
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000). You can also deploy the folder directly to any static web host.

## Controls

| Key | Action |
| --- | --- |
| W A S D | Steer |
| Space | Fire pulse cannons |
| Shift | Afterburn dash and proximity burst |
| X | Invulnerable somersault |
| V | Toggle copilot and chase views |
| Esc | Pause or resume |

## Project files

- `index.html` — game page and HUD
- `style.css` — visual design and responsive layout
- `game.js` — Three.js scene, flight controls, combat, waves, and effects

The game is intentionally dependency-light: Three.js is pinned to r160 through jsDelivr, and all ships, environments, portraits, and effects are drawn in code or CSS/SVG.
