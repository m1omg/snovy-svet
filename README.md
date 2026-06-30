# 🌙 Snový Svet (Dreamscape)

A 2D side-scrolling platformer where you are **Oliver**, a child who falls asleep and explores a strange, dreamlike world. Travel through **12 procedurally generated dream realms**, collect dream orbs, put enemies to sleep with a "dream beam", survive 3 boss fights, and reach the exit portal of each realm until you wake up.

> Built as a single self-contained `index.html` — vanilla JS, HTML5 Canvas 2D, Web Audio API. No libraries, no build step, no network. Runs offline.

🎮 **Play online:** https://m1omg.github.io/snovy-svet/

---

## ✨ Features

- **12 themed dream realms** — each with its own color palette, decorations, parallax background, and procedurally generated music scale (ethereal / melancholy / cosmic)
- **Player mechanics:**
  - Triple jump (3 jumps in a row, distinct SFX per jump #)
  - Wall slide & wall jump
  - Dash (with i-frames, damages enemies)
  - Ground pound (AoE damage on landing)
  - Dream beam (hold-to-fire, combo-scaled range)
- **5 enemy types** unlocked progressively — ghost, amoeba, shooter, jumper, flyer. Defeated enemies *sleep* and revive after a delay (they're pacified, not destroyed)
- **3 boss fights** on realms 4, 8, 12 — Shadow King, Dream Eater, Void Walker. Each has phased attacks; the exit portal is **locked** (sealed 🔒) until the boss is defeated
- **Procedural level generation** — solid, fading, moving, and hidden platforms; gaps scale with difficulty; orbs, hearts, checkpoints, and 1–2 secret areas per realm
- **Combo system** — collecting orbs in succession multiplies score; every 10 in a combo grants +1 life
- **Procedural Web Audio** — generative ambient music (3 scales per realm) + 15+ synthesized SFX, all built at runtime
- **Slovak (default) + English** localization toggle
- **3 difficulty presets** — Easy / Medium / Hard affecting lives, gravity, enemy count, beam energy, invincibility, etc.
- **Responsive design** — render resolution decoupled from display size; touch controls (swipe or D-Pad), 70% / 100% zoom for mobile, FPS counter toggle
- **Particle system** (capped at 150) — circles, sparks, stars, hearts, smoke; screen shake; neon "dreamcore" styling
- **Two distinct Oliver assets:**
  - `olivershaded.png` (688×619) — detailed illustration shown only on the intro screen
  - `oliver-ingame-sprite.png` (117×139) — small chibi sprite used for the gameplay character (credited to "Nero")

---

## 🎮 Controls

### Keyboard (desktop)
| Action | Key |
|---|---|
| Move | ← → / A D |
| Jump (triple) | ↑ / W / click |
| Dream beam (hold) | Space / Ctrl |
| Dash | Shift / E |
| Ground pound (in air) | ↓ / S |
| Pause | Esc / P |

### Touch (tablet / mobile)
- **Swipe mode** (default): swipe to move, swipe up = jump, swipe down = ground pound, two-finger tap = dash
- **D-Pad mode**: on-screen ▲▼◀▶ + action buttons (SKOK / LÚČA / DASH)

Switch control mode in the menu or pause screen.

---

## 🚀 Run

### Option 1: Play online
Open https://m1omg.github.io/snovy-svet/ in any modern browser.

### Option 2: Run locally
1. Clone this repo
2. Open `index.html` in your browser (Chrome / Firefox / Safari / Edge)

No server, no build step, no dependencies. It even works from `file://`.

### Option 3: Embed
Copy `index.html` + the two PNGs to any static host (GitHub Pages, Netlify, Vercel, S3, your own server).

---

## 📁 Project structure

```
snovy-svet/
├── index.html                  # The complete game (single file)
├── olivershaded.png            # 688×619 intro illustration
├── oliver-ingame-sprite.png    # 117×139 in-game chibi sprite
├── README.md                   # This file
├── LICENSE                     # MIT
└── snovy-svet-game-spec.md     # Original design spec (for reference)
```

---

## 🛠 Tech stack

- **Vanilla JavaScript** (ES6, IIFE-wrapped)
- **HTML5 Canvas 2D** for rendering
- **Web Audio API** for procedural music + SFX
- **Google Fonts** — Comfortaa (loaded from CDN)
- **No frameworks, no bundler, no dependencies**

---

## 🎨 Credits

- **Hero illustration** (`olivershaded.png`): by **Nero** 💙
- **In-game sprite** (`oliver-ingame-sprite.png`): chibi Oliver
- **Game design & code**: built from the spec by an AI assistant

---

## 📜 License

MIT — see [LICENSE](LICENSE).

The Oliver character illustrations are credited to their respective artists and are included in this repo for the purpose of running the game. If you fork this repo and replace the assets, please respect the original artists' wishes.
