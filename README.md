# 🌙 TouchyTouchy – Walk With Me

A browser-based interactive walking character experience set in a stylized night world. Click anywhere on the screen or use your keyboard to guide a pixel-art character through a glowing, animated landscape.

---

## ✨ Features

- **Click-to-Move** — Click anywhere in the world and the character walks smoothly to that point
- **Keyboard Movement** — Use `W A S D` or `↑ ↓ ← →` arrow keys for direct control
- **Directional Sprite Animation** — 4-frame walk cycles for all four directions (up, down, left, right)
- **Footprint Trail** — Glowing footprints fade out behind the character as it walks
- **Click Ripple Effect** — A ripple animation marks your click target
- **Animated Starfield** — 200 twinkling stars rendered on an HTML5 Canvas
- **Pulsing Moon** — A softly glowing moon with a CSS keyframe pulse animation
- **Parallax Mountains** — CSS-drawn far-background mountain silhouettes
- **Procedural Trees** — Randomly scaled layered-canopy trees injected at startup
- **HUD Overlay** — Live X/Y position, direction label, and a speed indicator bar
- **Fullscreen Mode** — Toggle fullscreen with a single button click
- **Clear Trail** — Instantly removes all footprints from the scene
- **Title Splash Screen** — Animated intro screen with instructions before play begins
- **Toast Notification** — Fade-out control hint shown for the first 5 seconds

---

## 🗂️ Project Structure

```
TouchyTouchy/
├── index.html          # All HTML, CSS, and JavaScript (single-file app)
└── images/
    ├── right_0.png     # Walk right — frame 0
    ├── right_1.png     # Walk right — frame 1
    ├── right_2.png     # Walk right — frame 2
    ├── right_3.png     # Walk right — frame 3
    ├── left_0.png      # Walk left  — frame 0
    ├── left_1.png      # Walk left  — frame 1
    ├── left_2.png      # Walk left  — frame 2
    ├── left_3.png      # Walk left  — frame 3
    ├── up_0.png        # Walk up    — frame 0
    ├── up_1.png        # Walk up    — frame 1
    ├── up_2.png        # Walk up    — frame 2
    ├── up_3.png        # Walk up    — frame 3
    ├── down_0.png      # Walk down  — frame 0
    ├── down_1.png      # Walk down  — frame 1
    ├── down_2.png      # Walk down  — frame 2
    └── down_3.png      # Walk down  — frame 3
```

---

## 🚀 Getting Started

No build step, no dependencies, no package manager required.

1. **Clone or download** the repository
2. **Open** `index.html` in any modern browser

```bash
# If you have VS Code with Live Server:
# Right-click index.html → "Open with Live Server"

# Or open directly in a browser:
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

> **Note:** The sprite images are loaded via relative paths (`images/*.png`). Make sure the `images/` folder stays alongside `index.html`.

---

## 🎮 Controls

| Input | Action |
|---|---|
| `Mouse Click` | Move character to clicked position |
| `W` / `↑` | Walk up |
| `S` / `↓` | Walk down |
| `A` / `←` | Walk left |
| `D` / `→` | Walk right |
| `⛶ Fullscreen` button | Toggle fullscreen mode |
| `✦ Clear Trail` button | Remove all footprints |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | Vanilla CSS (animations, gradients, glassmorphism) |
| Logic | Vanilla JavaScript (no frameworks) |
| Rendering | HTML5 Canvas (starfield) |
| Fonts | Google Fonts — *Orbitron*, *Inter* |

---

## 🎨 Design System

The visual theme is built around a deep-space night palette:

| Token | Value | Use |
|---|---|---|
| `--sky-top` | `#0f0c29` | Gradient sky top |
| `--sky-mid` | `#302b63` | Gradient sky mid |
| `--sky-bot` | `#24243e` | Gradient sky bottom |
| `--ground` | `#16213e` | Ground base |
| `--ground-top` | `#4834d4` | Ground border glow |
| `--accent` | `#a29bfe` | UI highlights & footprints |
| `--glow` | `#6c5ce7` | Buttons & speed bar |

---

## 📸 Sprite Format

Each directional walk animation consists of **4 frames** named:

```
{direction}_{frame}.png     e.g. right_0.png, left_3.png
```

- **Size:** Displayed at `80 × 120 px` with `background-size: contain`
- **Rendering:** `image-rendering: pixelated` for crisp pixel-art scaling
- **Frame Rate:** ~140 ms per frame (~7 fps walk cycle)

---

## 📄 License

This project is open for personal and educational use.
