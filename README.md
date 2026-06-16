# Oval Beam Kerf Offset

A browser-based tool for calculating and tracing accurate kerf offset for laser cutters with oval or asymmetric beams.

## What it does

Most laser cutters don't have a perfectly round beam — the beam is slightly oval, with different widths in the horizontal, vertical, and diagonal directions. Standard kerf offset tools assume a round beam and produce inaccurate results.

This tool accounts for the true oval shape of your beam, giving you accurate kerf offsets at every angle around your shape.

## Features

- **Accurate kerf offset tracing** — traces inner and outer kerf offset for SVG shapes
- **Oval beam support** — models your beam's true shape using width, height, and diagonal measurements
- **Blunt Corners mode** — removes sharp points from inlay shapes so they fit perfectly into pockets
- **Beam presets** — save your laser machine profiles for quick switching
- **Multiple path support** — processes all closed paths in a single SVG file in one go. A text inlay of 100 letters can be processed in a few seconds
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

### 3. Load your SVG

Load your SVG shape, then tap **Trace Kerf Offset**. Use the other buttons to remove small loops caused by corners, and select corner type.

### 4. Zoom

Zoom in to see minute detail of the offset paths.

### 5. Download

When you are happy with your results, choose which paths to download and download to your device/computer.

### Beam Presets

Open the HTML file in a text editor. Near the top of the code you will find a section clearly marked:

// LASER BEAM PRESETS — EDIT YOUR LASER SIZES HERE


Edit the name, width, height, and diagonal values to match your machines. 
*** Remember to SAVE before leaving text editor ***.
Now on next reload you can select your laser beam dimensions from the dropdown. 
Do not edit anything outside this section unless you know html

## Download

Download the latest version: [Oval Kerf Offset.html](https://github.com/Longjohn1/Oval-Beam-Kerf-Offset/releases/download/V1.0/Oval.Kerf.Offset.html)

Open it in any modern browser — no installation required.

## License

This project is licensed under the GNU General Public License v3.0 — see the [LICENSE](LICENSE) file for details.
