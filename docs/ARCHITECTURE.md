# Application architecture

- `index.html`: semantic application shell and accessible controls.
- `styles.css`: responsive desktop/mobile dashboard styling.
- `app.js`: minimal WebGL 2 renderer, camera, parametric geometry, analysis overlays and UI state.
- `data/app-data.js`: generated project data from CSV engineering outputs.
- `sw.js`: offline application-shell cache.
- `assets/downloads/`: downloadable engineering artefacts.

The application intentionally uses no npm build, framework, CDN or runtime dependency. GitHub Pages serves the files directly.
