# Geometry Dash

A fast-paced, browser-based arcade jump-and-fly platformer inspired by Geometry Dash. Guide your neon cube through 20 unique themed levels packed with spikes, blocks, jump orbs, and gravity-defying flight sections. Built with pure HTML5, CSS, and vanilla JavaScript — no dependencies, no build step.

🎮 **[Play Now](https://geometrydashjs.github.io)**

## Features

- 🎯 **20 unique levels** — each with its own neon color theme and increasing difficulty
- 🕹️ **Simple one-button controls** — tap the screen or press Space / Arrow Up to jump
- 🚀 **Multiple modes** — classic cube jumping and gravity-based flight sections via portals
- 💫 **Jump orbs** — mid-air boosts for extra momentum
- ⭐ **Star rating system** — earn 1–3 stars per level based on how few attempts you take
  - ★★★ — cleared in 1–2 tries
  - ★★☆ — cleared in 3–5 tries
  - ★☆☆ — 6+ tries
- 🏆 **Top 20 records** — your best runs saved with human-readable dates and times
- 🎉 **Congratulations screen** — celebrate beating all 20 levels with your total star count
- 📱 **Fully responsive** — works on desktop and mobile with touch support
- 💾 **Auto-save progress** — levels, stars, and records persist via `localStorage`
- 🎨 **Neon visuals** — smooth particles, glowing player, and animated backgrounds

## Controls

| Action | Desktop | Mobile |
|--------|---------|--------|
| Jump | `Space` or `↑` | Tap anywhere |
| Activate jump orb | Jump near the orb | Tap near the orb |

## Gameplay Tips

- **Timing is everything** — the game features coyote time (jump slightly after leaving a ledge) and jump buffering (press slightly early) to keep controls fair.
- **Forgiving hitboxes** — spikes only kill near their tips, and blocks only kill on real side impacts.
- **Land on blocks** — you can jump on top of blocks to reach new heights.
- **Watch for portals** — colored portals switch you between cube and flight mode.
- **Fewer attempts = more stars** — master a level to earn all three stars.

## Getting Started

No installation or build tools required. The entire game is a single self-contained HTML file.

### Play locally

1. Clone the repository:
   ```bash
   git clone https://github.com/geometrydashjs/geometrydashjs.github.io.git
   ```
2. Open the HTML file in your browser:
   ```bash
   cd geometrydashjs.github.io
   open index.html
   ```

That's it! No server, no npm, no dependencies.

### Host it yourself

Since it's a static site, you can host it anywhere — GitHub Pages, Netlify, Vercel, or any static file server.

## Technical Details

- **Rendering:** HTML5 Canvas with device-pixel-ratio scaling for crisp visuals on all displays
- **Level generation:** procedural, deterministic levels using a seeded `mulberry32` PRNG — the same level layout every time
- **Storage:** progress, stars, and records saved in `localStorage`
- **No dependencies:** 100% vanilla JavaScript, CSS, and HTML
- **Responsive HUD:** the progress bar and level info are positioned relative to the actual game viewport, correctly handling letterboxing on any aspect ratio

## Browser Support

Works in all modern browsers that support:
- HTML5 Canvas
- Pointer Events
- CSS `clamp()` and Flexbox/Grid
- `localStorage`

Tested on Chrome, Firefox, Safari, Edge, and Opera (including mobile).

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for bug fixes, new levels, themes, or features.

## License

MIT
