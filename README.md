# Space Engineer — Top-Down Game

A browser-based top-down game built with vanilla JS + Canvas.

## Files

```
index.html                    ← the whole game
GAME_MAP.png                  ← level map
Space_Engineer_Walk_Cycle.png ← character sprite sheet
walkable_space.png            ← collision mask (black = walkable)
```

## Controls

| Key | Action |
|-----|--------|
| ↑ / W | Move up |
| ↓ / S | Move down |
| ← / A | Move left |
| → / D | Move right |

## Hosting on GitHub Pages

1. Create a new GitHub repo (e.g. `space-engineer-game`)
2. Drop all 4 files into the root of the repo
3. Push to `main`
4. Go to **Settings → Pages**
5. Under *Source*, select **Deploy from a branch** → `main` → `/ (root)`
6. Hit **Save** — your game will be live at:
   `https://YOUR-USERNAME.github.io/space-engineer-game/`

## Tweaking

All config is at the top of `index.html` in the `// ─── CONFIG ───` block:

```js
const SPEED = 3;          // player movement speed
const CHAR_SCALE = 0.22;  // character size (increase to make bigger)
const MAP_SCALE = 0.75;   // map zoom (1.0 = full size, 0.5 = half)
const ANIM_FPS = 10;      // walk animation speed
```

To adjust starting position, change:
```js
let playerX = 300 * MAP_SCALE;
let playerY = 150 * MAP_SCALE;
```
