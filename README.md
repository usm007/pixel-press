# Pixel Press

Client-side exact file size optimizer & cropper. Single HTML file, zero dependencies, works offline — no uploads, everything stays in the browser.

Open `index.html` (serve over HTTP for best results, e.g. `python -m http.server`) — or use it as your PWA shell.

## Features

- **Exact target size** — set KB/MB (or tap a preset: 20 / 50 / 100 / 110 / 150 / 200 KB); quality is binary-searched, then dimensions shrink automatically until the file fits
- **Format detection & conversion** — input MIME sniffed from magic bytes (lying extensions caught); lossless PNG/BMP auto-convert to JPEG/WebP; explicit JPEG / WebP / PNG output with MIME verification
- **Smart PNG** — kept lossless when it fits, auto-converted to JPEG when it can't
- **PDF output** — single-page PDF wrapping the target-sized JPEG, zero dependencies
- **Crop** — drag on canvas, standard ratios (1:1, 4:3, 3:2, 16:9, 9:16, 4:5, 2:3), free mode
- **Edits** — rotate, flip H/V, straighten slider, manual 4-corner perspective (keystone) fix
- **Resolution control** — Width × Height inputs, blank = original, aspect always preserved
- **Bulk mode** — queue many files with per-file results and downloads
- **Side-by-side** input vs output comparison
