# DDpro Logo — SVG Badge (512×512)

A small fun side project by DeDynamics.pro:
a clean, scalable SVG version of the DDpro logo, built after a long (and slightly obsessive) debugging journey through CSS rendering quirks and browser artifacts.

This repository exists because:
- we enjoy understanding why things break
- we prefer simple, robust solutions
- and SVG turned out to be the most honest answer 😉

---

## What this is

- A single-file HTML + inline SVG logo
- Fixed size: 512 × 512
- No shadows, no hacks, no clipping artifacts
- Works reliably across browsers
- Easy to export to PNG, PDF, or embed directly

---

## Why SVG

During development we discovered that:
- CSS text + gradients + transforms can cause subtle rendering artifacts (“clipping”)
- different browsers rasterize transformed text differently
- SVG text with gradients and stroke is far more predictable

So this version:
- uses pure SVG shapes + text
- keeps layering explicit
- avoids GPU compositing issues entirely

Result: clean edges, stable output, zero surprises.

---

## Features

- Outer ring with subtle gradient
- Inner thin ring
- Dark radial disc
- Bold system sans-serif lettering
- Thick outline stroke for clear separation
- No external dependencies
- No JavaScript

---

## Font choice

To keep the logo portable and reproducible, this version uses a universal system font stack:

    system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif

This ensures:
- consistent behavior on Windows, macOS, and Linux
- no font licensing issues
- no missing-font surprises

(Previous Bauhaus-based experiments were intentionally dropped here.)

---

## Customisation

You can safely tweak:

- Stroke thickness:
    stroke-width="2.6"

- Stroke darkness:
    stroke="rgba(0,0,0,0.38)"

- Text size:
    font-size="240"

- Colors:
  Inside the <defs> section (linear & radial gradients)

All changes are local and predictable.

---

## Usage

- Open the HTML file directly in a browser
- Copy the <svg> block into any website
- Export to PNG using browser dev tools or design software
- Use as favicon / app icon / badge / branding element

---

## Philosophy

This repo is intentionally small.

It reflects how we like to work at DeDynamics.pro:
- understand the problem deeply
- strip away unnecessary complexity
- ship something stable and understandable
- have fun along the way

---

## License

MIT — do whatever you want, just don’t pretend you debugged this with fewer headaches than we did 😉

---

## About DeDynamics.pro

DeDynamics.pro is a creative-tech workshop exploring:
- design
- decentralisation
- AI
- photography
- and practical tools that actually work

This logo repo is just one playful artifact of that mindset.

