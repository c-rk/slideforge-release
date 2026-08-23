# SlideForge

A presentation maker that runs entirely in your browser. One HTML file, no backend, no accounts, no tracking.

Live: https://slideforge-dcs.pages.dev/

## Features

- Text, shapes, lines, arrows, images and LaTeX math on a drag and drop canvas
- Move, resize, rotate, group, snap to grid, undo and redo
- Paste images with Ctrl+V: screenshots, image files, or an image copied off a web page
- Export PNG at 1x up to 6x, either the current slide or every slide
- Export a standalone HTML slideshow that presents offline, with math and fonts built in
- Save as JSON and reopen later to keep editing
- Present mode with speaker notes, presenter view and a timer
- Print to PDF
- Per element animations and per slide transitions
- Slide templates, light and dark themes, touch support on phones and tablets

## Privacy

Everything stays on your machine. Slides are held in the tab's session storage and are erased when you close it. Nothing is ever uploaded.

## Running it

Open `index.html` in any modern browser, or serve the folder from any static host.

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `tex-svg-full.js` | Self hosted MathJax, so math needs no CDN |
| `_headers` | Security headers for Cloudflare Pages |

To deploy on Cloudflare Pages: create a Pages project, point it at this repo, leave the build command empty and set the output directory to `/`.
