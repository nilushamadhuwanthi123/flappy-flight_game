# Flappy Flight

A polished Flappy Bird clone built entirely in vanilla JavaScript and the Canvas API — no frameworks, no build step, no external dependencies. Every visual, from the bird to the pipes to the scrolling ground, is drawn with Canvas primitives; there are no image or font assets to load.

This project demonstrates a fixed-timestep game loop architecture decoupled from rendering, device-pixel-ratio-aware responsive canvas rendering, unified keyboard/touch/mouse input handling, persisted state via localStorage, and accessibility considerations like reduced-motion support and visible focus states.

## Features
- Smooth fixed-timestep game loop (requestAnimationFrame + accumulator), so physics stays consistent across frame rates
- Responsive, device-pixel-ratio-aware canvas rendering that adapts to desktop and mobile viewports
- Keyboard (Space / Arrow Up) and touch/click/tap controls, unified through a single input entry point
- Circle-vs-rectangle collision detection against pipes, ground, and ceiling
- Persistent high score saved to `localStorage`, shown on both the start and game-over screens
- Start screen, in-game score HUD, and a game-over screen with score, best score, and one-tap restart
- Reduced-motion support (`prefers-reduced-motion`) that dials back background parallax and scroll effects while keeping core gameplay intact
- Dark, warm-gold visual theme with hand-drawn bird (body, wing, eye, beak) and layered pipe/ground shading — no external image or font assets

## Run it
Just open `index.html` in a browser — no build step, no install.

## Live version
Play it here: https://nilushamadhuwanthi123.github.io/flappy-flight_game/
