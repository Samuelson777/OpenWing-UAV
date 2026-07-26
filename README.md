# OpenWing-UAV Live 3D GitHub Pages App

A no-build, dependency-free WebGL application that presents the OpenWing-UAV engineering digital thread from Version 0.1 through Version 0.9.

## Run locally

Open `index.html` directly, or use a local server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a new GitHub repository.
2. Copy every file from this package into the repository root.
3. Push to the `main` branch.
4. Open **Settings → Pages** and select **GitHub Actions**.
5. The included workflow deploys the static site.

## Features

- Parametric NACA 4412 full-wing WebGL model
- Dihedral and washout geometry
- Internal ribs, spars, joiner, servo and ailerons
- Version timeline from 0.1 to 0.9
- Aerodynamic load and polar visualisation
- Equivalent-beam FEA deformation and modal animation
- Optimisation candidate comparison
- Prototype proof-load and sensor layout
- Digital-thread visualisation
- Responsive desktop/mobile interface
- Screenshot export, guided tour and keyboard shortcuts
- Offline application shell after first HTTP load

## Accuracy boundary

The live geometry follows the project baseline dimensions. Aerodynamic and structural overlays use the generated lifting-line and equivalent-beam datasets included in the project. The app is a visual engineering portfolio and does not replace native CAD, CFD, FEA or physical validation.
