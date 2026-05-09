# Loading Bars

A hand-crafted collection of 20 unique CSS loading animations — 10 bar/linear loaders and 10 circular loaders — built with pure HTML and CSS. No JavaScript libraries, no animation frameworks, no external dependencies. Every animation is driven entirely by CSS `@keyframes`, `::before`/`::after` pseudo-elements, and carefully tuned `animation-delay` values.

---

## What This Project Does

This repository contains 2 standalone HTML files, each showcasing 10 distinct loading animation styles on a dark background. The files are designed as a ready-to-use reference collection — each animation is numbered, isolated in its own card, and can be copied directly into any project.

---

## Files Included

### 1. Bar & Linear Loaders — `First_Loading_Bars.html`

10 loading animations based on horizontal bars, progress indicators, and geometric shapes — all displayed in a responsive grid layout.

**Animations included:**

**1. Neon Wave** — A glowing cyan light sweeps left to right across a thin horizontal bar using a `linear-gradient` and `translateX` animation.

**2. Pixel Progress** — 8 rectangular segments pulse from dim to pink in a staggered sequence using `animation-delay`, creating a wave-like fill effect.

**3. Orbital Loader** — Two concentric circular borders spin in opposite directions at different speeds using `::before` and `::after`. The inner ring uses `animation-direction: reverse`.

**4. Liquid Fill** — A blue-to-teal gradient bar slides in from the left and retracts, looping in an ease-in-out fill motion.

**5. Dot Matrix** — 5 green dots pulse in size and opacity with staggered delays, creating a breathing wave effect.

**6. Glitch Bar** — A pink block slides across a container in 8 stepped jumps (`animation-timing-function: steps(8)`) with a green scanning line moving independently, simulating a glitch effect.

**7. Neon Rings** — 3 concentric rings, each with a partial border visible on one side, rotate at different speeds and directions in green, pink, and blue.

**8. Barcode Loader** — 8 vertical bars scale up and change color in a staggered odd/even pattern, resembling a barcode being scanned.

**9. Circuit Loader** — Two small squares pulse at opposite corners while a connecting line animates between them, mimicking a circuit board signal trace.

**10. Gradient Flow** — A multi-color gradient (pink → green → blue → cyan) flows continuously left to right across a thin bar using `background-position` animation on a 400%-wide gradient.

**Additional interaction:** Every card lifts (`translateY(-5px) scale(1.02)`) on hover via a JavaScript event listener applied uniformly to all cards.

---

### 2. Circle Loaders — `Second_Loading_Bars.html`

10 loading animations based on circular and orbital motion — displayed in a responsive `auto-fit` grid.

**Animations included:**

**1. Simple Spinner** — A classic circular border spinner with a blue top border rotating continuously at 1s linear speed.

**2. Dot Circle** — A single green glowing dot orbits a circular path using a combined `rotate → translateY → rotate` transform trick to keep the dot upright while it orbits.

**3. Pulse Rings** — Two concentric circles scale from 0.5x to 1.5x while fading out in a staggered loop, creating an outward ripple effect.

**4. Neon Circle** — A circular div with a transparent border and a multicolor gradient applied via `border-box` background clipping rotates continuously, revealing the gradient as a spinning arc.

**5. Clock Loader** — A circular border with a single green hand (`::before` pseudo-element) anchored at the center rotates around a fixed point like a clock hand.

**6. Orbit Dots** — 4 orange dots orbit a circular path with staggered delays and decreasing opacity as they trail, creating a comet-tail appearance.

**7. Gear Loader** — Two concentric circular borders each with top and bottom segments visible (`border-top-color` / `border-bottom-color`) rotate in opposite directions at different speeds.

**8. Circle Dash** — A circle with only 2 of 4 border sides colored spins at 1s linear speed, producing a classic dashed ring spinner.

**9. Bubble Circle** — 4 blue dots positioned at the top, right, bottom, and left of a circle pulse in size and opacity with 0.5s staggered delays.

**10. Infinity Circle** — A `conic-gradient` (transparent → pink → cyan → orange → transparent) rotates continuously, masked by a `radial-gradient` that hides the center, producing a spinning arc with a color gradient.

---

## Tech Stack

| Technology | Role |
|---|---|
| HTML5 | Structure and layout of animation cards |
| CSS3 | All animations via `@keyframes`, `transform`, `animation-delay`, pseudo-elements |
| JavaScript (Vanilla) | Hover lift effect on cards in `First_Loading_Bars.html` only |

**CSS techniques used across both files:**
- `@keyframes` for all motion
- `::before` / `::after` pseudo-elements to add animated layers without extra HTML
- `animation-delay` for staggered sequencing
- `animation-direction: reverse` for counter-rotation
- `animation-timing-function: steps()` for stepped/glitch motion
- `conic-gradient` and `radial-gradient` masking for arc effects
- `background-clip: border-box` + transparent background for gradient borders

---

## Project Structure

```
Loading_Bars/
├── First_Loading_Bars.html    # 10 bar/linear/geometric loading animations
└── Second_Loading_Bars.html   # 10 circular/orbital loading animations
```

---

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/tripathipawan/Loading_Bars.git
   ```
2. Open `First_Loading_Bars.html` or `Second_Loading_Bars.html` directly in any modern browser — no server, no build step, no dependencies to install.

---

## Repository

[https://github.com/tripathipawan/Loading_Bars](https://github.com/tripathipawan/Loading_Bars)
