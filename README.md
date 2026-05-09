# Loading Bars

A hand-crafted collection of 20 unique CSS loading animations — 10 bar/linear loaders and 10 circular loaders — built entirely with HTML and CSS. No JavaScript animation libraries, no external frameworks, no dependencies of any kind. Every animation is driven purely by CSS `@keyframes`, `::before` / `::after` pseudo-elements, `animation-delay` staggering, and carefully chosen easing functions.

---

## What This Project Does

This repository contains 2 standalone HTML files, each showcasing 10 distinct loading animation styles on a dark background. Every animation is isolated in its own card, numbered, and immediately copy-paste ready. The files are designed as a practical reference and demonstration of what is achievable with CSS alone.

---

## Files Included

### 1. Bar & Linear Loaders — `First_Loading_Bars.html`

10 loading animations based on horizontal bars, progress indicators, orbital rings, and geometric shapes — displayed in a responsive `auto-fill` CSS Grid with `minmax(300px, 1fr)` column sizing.

**Animation 1 — Neon Wave**
A glowing cyan light sweeps left to right across a thin 4px horizontal bar. Implemented using a `::before` pseudo-element with `background: linear-gradient(90deg, transparent, #00f3ff, transparent)` that translates from `-100%` to `100%` using `translateX` on a 2s linear infinite loop.

**Animation 2 — Pixel Progress**
8 rectangular segments arranged in a flex row pulse from a dim background to `#ff2d75` in a staggered wave. Each segment uses `animation-delay` values from `0s` to `1.4s` (increments of `0.2s`) on a shared `pixel-load` keyframe.

**Animation 3 — Orbital Loader**
Two concentric circular borders spin in opposite directions at different speeds using `::before` and `::after`. The outer ring uses `border-top-color: #00ff88` at 1.5s; the inner ring is 70% the size, uses `border-top-color: #ff2d75`, runs at 1s, and has `animation-direction: reverse`.

**Animation 4 — Liquid Fill**
A blue-to-teal gradient bar (`background: linear-gradient(90deg, #0088ff, #00ffcc)`) slides in from the left and retracts on a 2s `ease-in-out` loop. The bar starts at `translateX(-100%)`, reaches `translateX(0)` at 50%, and returns — creating the impression of a liquid filling and emptying.

**Animation 5 — Dot Matrix**
5 green dots pulse in size (from `scale(0.5)` to `scale(1.2)`) and opacity (from `0.3` to `1`) with `0.2s` staggered delays, producing a breathing wave from left to right.

**Animation 6 — Glitch Bar**
A pink (`#ff2d75`) block moves across a container in exactly 8 stepped jumps using `animation-timing-function: steps(8)` — going from `left: 0` to `left: 60%` and back. Simultaneously, a separate green scanning line sweeps across the full width using a second `::after` animation, producing a glitch effect.

**Animation 7 — Neon Rings**
3 concentric rings, each with only one side of their border colored (`border-color: transparent #00ff88 transparent transparent`), rotate at 2s, 1.5s (reversed), and 1s respectively. Each ring is positioned absolutely at a different percentage of the container.

**Animation 8 — Barcode Loader**
8 vertical bars scale up on the Y-axis (`scaleY`) and change color from a dim background to `#0088ff` in a staggered odd/even pattern. Odd-positioned bars have a `0.3s` additional delay, creating a visual resemblance to a barcode scanner moving across a barcode.

**Animation 9 — Circuit Loader**
Two small squares (`::before` and `::after`) positioned at opposite corners pulse in scale and opacity on a 1.2s loop with `0.6s` offset. A `<span>` child element animates its width from `0` to `80px` and back, connecting the two squares like a signal trace on a circuit board.

**Animation 10 — Gradient Flow**
A 4-color gradient (`#ff2d75 → #00ff88 → #0088ff → #00f3ff`) is defined at `background-size: 400% 100%` and animated by shifting `background-position` from `100% 0` to `-300% 0` on a 2s linear infinite loop, making the colors appear to flow continuously in one direction.

**Bonus — Hover Lift Effect**
A JavaScript `mouseenter`/`mouseleave` listener is applied to all cards, lifting each card by `translateY(-5px) scale(1.02)` on hover and resetting it on leave.

---

### 2. Circle Loaders — `Second_Loading_Bars.html`

10 loading animations based on circular shapes, orbiting elements, and radial motion — displayed in a `auto-fit` CSS Grid.

**Animation 1 — Simple Spinner**
A circular `div` with `border: 8px solid rgba(0,100,255,0.1)` and `border-top: 8px solid #0066ff` rotates at 1s linear speed. The classic baseline spinner.

**Animation 2 — Dot Circle**
A single green glowing dot orbits a circular path while staying upright. This uses a combined transform trick: `rotate(Xdeg) translateX(-50%) translateY(40px) rotate(-Xdeg)` — the outer rotation moves the dot around the center, and the counter-rotation keeps the dot itself from spinning.

**Animation 3 — Pulse Rings**
Two concentric circles (`::before` and `::after`) scale from `0.5x` to `1.5x` while their opacity fades from `1` to `0`, looping on a 2s timeline with 1s offset. The result is a continuous outward ripple effect, like a radar ping.

**Animation 4 — Neon Circle**
A circular `div` with a transparent border uses `background-clip: border-box` combined with a `linear-gradient(45deg, #ff00cc, #00ffff)` applied as the background source for the border area. Rotating this div at 2s linear makes the gradient appear to spin around the ring.

**Animation 5 — Clock Loader**
A circular border acts as the clock face. A `::before` pseudo-element sized `4px × 30px` is positioned at the center with `transform-origin: 0 0` and rotates a full 360° on a 2s linear loop, behaving exactly like a clock hand sweeping around.

**Animation 6 — Orbit Dots**
4 orange dots each orbit the center using `rotate(Xdeg) translateX(40px)` with staggered `0.3s` delays. The dots' opacity fades from `1` to `0.3` as they trail, giving a comet-tail appearance.

**Animation 7 — Gear Loader**
Two concentric rings each have `border-top-color` and `border-bottom-color` set (leaving left and right sides transparent), so only two opposing arcs are visible on each ring. The outer ring (red) and inner ring (green) spin in opposite directions at 1.5s and 1s respectively, resembling interlocking gears.

**Animation 8 — Circle Dash**
A circle with only `border-top` and `border-right` colored (the other two sides transparent) spins at 1s linear speed, producing a classic two-segment arc spinner.

**Animation 9 — Bubble Circle**
4 blue dots are positioned at the top, right, bottom, and left of a circle using absolute positioning. They pulse in `scale` and `opacity` with `0.5s` staggered delays — North, East, South, West each peaks at a different moment.

**Animation 10 — Infinity Circle**
A `conic-gradient(transparent, #ff00cc, #00ffff, #ffaa00, transparent)` is applied to a circular `div`. The center is masked out using `mask: radial-gradient(circle at center, transparent 55%, black 56%)`, leaving only a spinning arc ring visible. The gradient rotates at 2s linear speed, making the arc appear to flow with color.

---

## Tech Stack

| Technology | Role |
|---|---|
| HTML5 | Card containers, loader markup, page layout |
| CSS3 | All 20 animations via `@keyframes`, pseudo-elements, `animation-delay`, transforms |
| JavaScript (Vanilla) | Hover lift effect on cards in `First_Loading_Bars.html` only — 8 lines total |

**CSS techniques demonstrated across both files:**
- `@keyframes` for all motion
- `::before` / `::after` pseudo-elements to layer animated elements without extra HTML
- `animation-delay` for staggered timing sequences
- `animation-direction: reverse` for counter-rotation
- `animation-timing-function: steps(N)` for stepped / glitch-style motion
- `conic-gradient` + `mask: radial-gradient` for arc spinner effects
- `background-clip: border-box` + transparent background for gradient borders
- `transform-origin` manipulation for clock hand and spoke rotations

---

## Project Structure

```
Loading_Bars/
├── First_Loading_Bars.html    # 10 bar, wave, ring, and geometric loading animations
└── Second_Loading_Bars.html   # 10 circular, orbital, and radial loading animations
```

---

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/tripathipawan/Loading_Bars.git
   ```
2. Open `First_Loading_Bars.html` or `Second_Loading_Bars.html` directly in any modern browser — no build step, no server, nothing to install.

---

## Repository

[https://github.com/tripathipawan/Loading_Bars](https://github.com/tripathipawan/Loading_Bars)
