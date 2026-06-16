# Oval Beam Kerf Offset

A browser-based tool for calculating and tracing accurate kerf offsets for laser cutters with oval or asymmetric beams.

## What it does

Most laser cutters don't have a perfectly round beam — the beam is slightly oval, with different widths in the horizontal, vertical, and diagonal directions. Standard kerf offset tools assume a round beam and produce inaccurate results.

This tool accounts for the true oval shape of your beam, giving you accurate kerf offsets at every angle around your shape.

## Features

- **Accurate kerf offset tracing** — traces inner and outer kerf offsets for SVG shapes
- **Oval beam support** — models your beam's true shape using width, height, and diagonal measurements
- **Blunt Corners mode** — removes sharp points from inlay shapes so they fit perfectly into pockets
- **Beam presets** — save your laser machine profiles for quick switching

- **No installation** — runs entirely in your browser, open the HTML file and go

## How to use

### 1. Measure your beam

Cut a test octagon on your laser and measure it with calipers across the width, height, and diagonal.

For example — a 20mm octagon that measures:
- Height: 19.95mm
- Width: 19.91mm  
- Diagonal: 19.925mm

Subtract each from 20mm to get the beam radius, then multiply by 2 for the full beam size:
- Height: **0.10mm**
- Width: **0.18mm**
- Diagonal: **0.15mm**

### 2. Enter your beam dimensions

Enter these three values into the beam dimension boxes at the top of the tool.

### 3. Load your SVG and trace

Load your SVG shape, then tap  **Trace Kerf Offset**.

### 4. Customise beam presets

Open the HTML file in a text editor. At the very top of the code you will find a section clearly marked:

```
// LASER BEAM PRESETS — EDIT YOUR LASER SIZES HERE
```

Edit the name, width, height, and diagonal values to match your machines. Do not edit anything outside this section.

## Download

Download the latest version: [`75_open_source_licence_added.html`](75_open_source_licence_added.html)

Open it in any modern browser — no installation required.

## License

This project is licensed under the GNU General Public License v3.0 — see the [LICENSE](LICENSE) file for details.
