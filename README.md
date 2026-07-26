# OpenWing-UAV

**An open, parametric, multidisciplinary UAV-wing engineering project integrating CAD, CAM, aerodynamics, structural simulation, optimisation, prototype validation, automation, and an interactive 3D web application.**

**Author:** Samuelson G
**Current development stage:** Version 0.9 digital thread
**Target release:** Version 1.0 reproducible engineering baseline

[![Project Status](https://img.shields.io/badge/status-prototype%20validation-orange)](#project-status)
[![Version](https://img.shields.io/badge/version-0.9.0-blue)](#development-history)
[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/Samuelson777/OpenWing-UAV/blob/main/LICENSE)
[![GitHub Pages](https://img.shields.io/badge/live%203D%20app-GitHub%20Pages-purple)](https://samuelson777.github.io/OpenWing-UAV/)
[![Engineering](https://img.shields.io/badge/domain-aerospace%20engineering-0b7285)](#project-overview)

---

## Table of Contents

* [Project Overview](#project-overview)
* [Project Objectives](#project-objectives)
* [Baseline Wing Specification](#baseline-wing-specification)
* [Key Features](#key-features)
* [Development History](#development-history)
* [Engineering Workflow](#engineering-workflow)
* [CAD and Structural Architecture](#cad-and-structural-architecture)
* [Aerodynamic Analysis](#aerodynamic-analysis)
* [Structural Simulation](#structural-simulation)
* [Optimisation](#optimisation)
* [Prototype Validation](#prototype-validation)
* [Live 3D Application](#live-3d-application)
* [Tutorial Drawings](#tutorial-drawings)
* [Repository Structure](#repository-structure)
* [Available File Formats](#available-file-formats)
* [Software Requirements](#software-requirements)
* [Getting Started](#getting-started)
* [Running the GitHub Pages App](#running-the-github-pages-app)
* [SOLIDWORKS 2023 Workflow](#solidworks-2023-workflow)
* [OpenVSP Workflow](#openvsp-workflow)
* [Python Automation](#python-automation)
* [Validation and Reproducibility](#validation-and-reproducibility)
* [Known Limitations](#known-limitations)
* [Project Status](#project-status)
* [Conclusion](#conclusion)
* [Future Enhancements](#future-enhancements)
* [Roadmap](#roadmap)
* [Safety Notice](#safety-notice)
* [Contributing](#contributing)
* [Citation](#citation)
* [License](#license)
* [Author](#author)

---

## Project Overview

OpenWing-UAV is an open-source engineering project focused on the complete digital development of a modular uncrewed-aircraft wing.

The project begins with a parametric aerodynamic layout and progressively integrates:

* Airfoil generation
* Wing planform design
* Dihedral and washout
* Internal spars and ribs
* Modular wing-joiner architecture
* Aileron and servo installation
* CAD and neutral-file generation
* CAM preparation
* OpenVSP and aerodynamic modelling
* Static structural analysis
* Root-joint and contact analysis
* Modal and buckling studies
* Fatigue and nonlinear-analysis planning
* Multidisciplinary optimisation
* Prototype proof and ultimate testing
* FEA-to-experiment correlation
* Repository automation
* Interactive browser-based 3D visualisation

The project is intended to demonstrate a complete aerospace engineering workflow that can be developed on a home PC and shared through an open-source GitHub repository.

---

## Project Objectives

The primary objectives of OpenWing-UAV are to:

1. Develop a modular UAV wing using a traceable parametric design process.
2. Connect aerodynamic geometry with internal structural architecture.
3. Produce reviewable CAD, neutral geometry, drawings, and manufacturing files.
4. Transfer aerodynamic loads into structural simulation cases.
5. Evaluate strength, displacement, buckling, vibration, joints, and control-system loads.
6. Optimise the design for mass, stiffness, stability, and manufacturability.
7. Define a safe and measurable physical-validation programme.
8. Automate repository validation, manifests, dashboards, and documentation.
9. Present the entire project through an interactive GitHub Pages application.
10. Establish a reusable framework for future UAV and aerospace projects.

---

## Baseline Wing Specification

| Parameter                        |            Value |
| -------------------------------- | ---------------: |
| Aircraft mass                    |           2.5 kg |
| Full wing span                   |         1,200 mm |
| Semi-span                        |           600 mm |
| Root chord                       |           240 mm |
| Tip chord                        |           160 mm |
| Wing area                        |         0.240 m² |
| Aspect ratio                     |              6.0 |
| Taper ratio                      |            0.667 |
| Airfoil                          |        NACA 4412 |
| Dihedral                         | 3° per half-wing |
| Midspan washout                  |              −1° |
| Tip washout                      |              −2° |
| Cruise speed                     |           15 m/s |
| Positive limit load              |           +3.5 g |
| Negative limit load              |           −1.5 g |
| Ultimate load factor             |              1.5 |
| Positive ultimate half-wing load |         64.356 N |
| Negative ultimate half-wing load |         27.581 N |

### Coordinate System

The primary SOLIDWORKS coordinate convention is:

```text
X-axis: spanwise
Y-axis: chordwise
Z-axis: vertical
Root plane: X = 0
```

---

## Key Features

### Parametric Geometry

* NACA 4412 airfoil generation
* Root, midspan, and tip airfoil profiles
* Tapered wing planform
* Equation-driven chord variation
* 3° dihedral
* Progressive washout
* Quarter-chord twist reference
* Configurable span, chord, and structural dimensions

### Internal Structure

* Main spar at approximately 30% chord
* Rear spar at approximately 70% chord
* Upper and lower spar caps
* Multiple structural rib stations
* Root support ribs
* Root web doubler
* Joiner box
* Rear anti-rotation pin
* Skin shell
* Servo bay
* Wiring channel
* Removable tip architecture

### Control System

* Outboard aileron
* Three hinge stations
* Servo tray
* Servo-arm and control-horn relationship
* Pushrod load calculations
* Positive and negative control deflections
* Servo-stall structural load case

### Engineering Validation

* Positive ultimate load case
* Negative ultimate load case
* Gust-load screening
* Ground-handling loads
* Tip torsion
* Local skin-pressure loads
* Root contact and bearing studies
* Modal analysis
* Buckling analysis
* Fatigue planning
* Nonlinear post-buckling sensitivity
* Aileron, hinge, and servo validation

---

## Development History

### Version 0.1 — Parametric Wing Foundation

* Established project repository
* Defined baseline aircraft and wing requirements
* Generated NACA 4412 airfoil coordinates
* Created root, midspan, and tip profiles
* Established coordinate systems and modelling conventions

### Version 0.2 — External Wing Geometry

* Created wing stations
* Applied taper, dihedral, and washout
* Constructed guide curves
* Generated boundary surfaces
* Formed the aerodynamic wing envelope

### Version 0.3 — Internal Structure and Assembly

* Added main and rear spars
* Added spar caps
* Defined rib stations
* Added root support structure
* Created joiner and anti-rotation-pin architecture
* Added servo bay, hinges, wiring channel, and aileron

### Version 0.4 — Drawings and Manufacturing Preparation

* Produced manufacturing drawings
* Prepared rib and spar DXF profiles
* Developed joiner CAM concepts
* Added additive-manufacturing components
* Prepared STEP, STL, and 3MF outputs
* Added assembly and manufacturing documentation

### Version 0.5 — Aerodynamic Analysis

* Defined OpenVSP wing geometry
* Prepared VSPAERO analysis workflow
* Developed angle-of-attack sweeps
* Generated spanwise aerodynamic loads
* Added aileron-effectiveness studies
* Added XFOIL airfoil-polars workflow
* Created preliminary performance envelopes

### Version 0.6 — Structural Multiphysics Validation

* Positive and negative static analyses
* Mesh-convergence planning
* Root-interface validation
* Modal analysis
* Buckling analysis
* Rotating-excitation comparison
* Gust and handling load cases
* Fatigue mission-spectrum templates
* Aileron, hinge, and servo analysis
* Nonlinear post-buckling planning

### Version 0.7 — Optimisation and Trade Studies

* Defined design variables
* Created goals and constraints
* Separated beam, skin/rib, and root optimisation
* Added lightweight, balanced, and high-stiffness candidates
* Developed Pareto-ranking workflow
* Added manufacturing-complexity scoring
* Added uncertainty and robustness studies

### Version 0.8 — Prototype Validation

* Defined material-coupon tests
* Created spar and root-joint test plans
* Added aileron and servo tests
* Developed positive and negative proof-load procedures
* Developed sacrificial ultimate-load procedures
* Added modal-impact testing
* Added FEA-to-experiment correlation templates
* Added controlled model-updating procedures

### Version 0.9 — Digital Thread and Automation

* Created GitHub-ready repository structure
* Added CSV schema validation
* Added automated repository checking
* Added SHA-256 release manifests
* Added GitHub Actions workflows
* Added a responsive live 3D GitHub Pages application
* Added interactive aerodynamic, structural, and manufacturing views
* Added project dashboards and downloadable assets

---

## Engineering Workflow

The project follows this connected workflow:

```text
Requirements
    ↓
Parametric airfoil and planform
    ↓
External aerodynamic geometry
    ↓
Internal spars, ribs, skin, and joints
    ↓
Control-system integration
    ↓
Manufacturing drawings and neutral exports
    ↓
Aerodynamic analysis
    ↓
Structural simulation
    ↓
Optimisation
    ↓
Prototype testing
    ↓
FEA-to-test correlation
    ↓
Controlled model update
    ↓
Reproducible engineering release
```

---

## CAD and Structural Architecture

### Airfoil Stations

| Station | Spanwise position |  Chord | Dihedral rise | Twist |
| ------- | ----------------: | -----: | ------------: | ----: |
| Root    |              0 mm | 240 mm |          0 mm |    0° |
| Midspan |            300 mm | 200 mm |      15.72 mm |   −1° |
| Tip     |            600 mm | 160 mm |      31.45 mm |   −2° |

### Rib Stations

The baseline rib architecture uses stations near:

```text
0, 25, 75, 150, 225, 300, 330, 390, 450, 510, 570, 600 mm
```

### Spar Dimensions

| Component             | Baseline dimension |
| --------------------- | -----------------: |
| Main spar web         |             1.5 mm |
| Rear spar web         |             1.2 mm |
| Main spar caps        |           6 × 3 mm |
| Rear spar caps        |           4 × 2 mm |
| Standard ribs         |             2.0 mm |
| Root ribs             |             3.0 mm |
| Aileron boundary ribs |             2.5 mm |
| Wing skin             |             1.0 mm |
| Aileron skin          |             0.8 mm |

### Joiner System

| Component          |   Baseline dimension |
| ------------------ | -------------------: |
| Joiner blade       |            18 × 4 mm |
| Insertion length   | 150 mm per half-wing |
| Full joiner length |               300 mm |
| Rear pin diameter  |                 6 mm |
| Rear-pin insertion |  60 mm per half-wing |
| Joiner clearance   |      0.20 mm nominal |

---

## Aerodynamic Analysis

The aerodynamic workflow includes:

* NACA 4412 profile generation
* OpenVSP geometry construction
* VSPAERO lifting-surface analysis
* Angle-of-attack sweeps
* Spanwise lift-distribution export
* Cruise-load mapping
* Aileron-effectiveness assessment
* XFOIL low-Reynolds-number polar generation
* Preliminary stall and performance estimation

Reference aerodynamic outputs include:

```text
OWU_LiftingLine_AlphaSweep.csv
OWU_LiftingLine_Cruise_SpanLoads.csv
```

The included lifting-line and potential-flow results are preliminary engineering references. They do not replace viscous CFD, wind-tunnel testing, or flight-test correlation.

---

## Structural Simulation

The structural workflow includes:

### Static Studies

* Positive ultimate manoeuvre
* Negative ultimate manoeuvre
* Positive gust
* Negative gust
* Wingtip handling
* Wingtip torsion
* Servo stall
* Aileron hinge moment
* Local skin pressure

### Local Studies

* Root joiner
* Joiner box
* Rear pin
* Adhesive interfaces
* Spar-cap and web transitions
* Hinge pins and lugs
* Servo tray and mounting bosses

### Dynamic Studies

* Unloaded modal analysis
* Prestressed modal analysis
* Bending and torsional mode classification
* Motor and propeller excitation mapping
* Blade-pass-frequency comparison

### Stability Studies

* Positive global buckling
* Negative global buckling
* Upper-skin local buckling
* Lower-skin local buckling
* Main-web buckling
* Rear-web buckling
* Imperfection sensitivity
* Nonlinear post-buckling response

Reference neutral results include:

```text
OWU_BeamFEA_PositiveUltimate.csv
OWU_BeamFEA_NegativeUltimate.csv
OWU_BeamFEA_Modal.csv
OWU_BeamFEA_PositiveUltimate.vtk
OWU_Equivalent_Wing_Beam.inp
```

These reference results are based on simplified neutral models and are not presented as completed SOLIDWORKS Simulation certification results.

---

## Optimisation

The Version 0.7 optimisation workflow divides the problem into manageable studies.

### Beam Sizing

Variables include:

* Main-web thickness
* Main-cap width
* Main-cap thickness
* Rear-web thickness
* Rear-cap width
* Rear-cap thickness

### Skin and Rib Stability

Variables include:

* Skin thickness
* Standard rib thickness
* Sparse, baseline, or dense rib layout

### Root and Joiner Sizing

Variables include:

* Joiner height
* Joiner thickness
* Joiner-box wall thickness
* Root-doubler length
* Root-doubler thickness

### Candidate Designs

Three principal candidate families are considered:

* Lightweight
* Balanced
* High-stiffness

### Optimisation Criteria

* Minimum mass
* Tip displacement
* Tip twist
* Spar strength
* Joiner strength
* Composite failure index
* Buckling load factor
* First bending frequency
* First torsional frequency
* Manufacturing complexity
* CAD rebuild success
* Uncertainty sensitivity

A Python ranking script identifies feasible and Pareto-optimal candidates.

---

## Prototype Validation

The planned physical-validation programme includes:

### Material Tests

* Skin laminate coupons
* Spar-cap coupons
* Plywood and web coupons
* Adhesive lap joints
* Printed-material orientation tests
* Hinge-bearing coupons

### Subcomponent Tests

* Main-spar four-point bending
* Root-joiner bending and torsion
* Aileron and hinge loading
* Servo-stall testing
* Hinge-cycle testing

### Full-Wing Tests

| Test                 | Half-wing target |
| -------------------- | ---------------: |
| Positive limit proof |         42.904 N |
| Negative limit proof |         18.387 N |
| Positive ultimate    |         64.356 N |
| Negative ultimate    |         27.581 N |

### Modal Testing

* Impact-hammer excitation
* Accelerometer measurements
* Frequency-response functions
* First bending mode
* First torsional mode
* Damping estimates
* FEA frequency correlation

### Correlation Targets

| Measurement               | Initial target |
| ------------------------- | -------------: |
| Tip displacement          |     ≤10% error |
| Midspan displacement      |     ≤10% error |
| Spar-cap strain           |     ≤15% error |
| Tip twist                 |     ≤15% error |
| Root rotation             |     ≤15% error |
| First bending frequency   |      ≤5% error |
| First torsional frequency |      ≤7% error |

These are project-level correlation targets, not regulatory requirements.

---

## Live 3D Application

The project includes a standalone GitHub Pages application built with HTML, CSS, and JavaScript.

### Features

* Interactive 3D wing model
* Orbit, pan, and zoom
* Isometric, front, and top views
* Version timeline from v0.1 to v0.9
* External aerodynamic geometry
* Internal rib and spar structure
* Joiner and root-system visualisation
* Aileron and servo views
* Aerodynamic span-load vectors
* Structural deformation display
* Modal animation
* Optimisation comparison
* Prototype-test visualisation
* Digital-thread dashboard
* Screenshot export
* Responsive mobile layout
* Software-rendered fallback where WebGL is unavailable

### GitHub Pages Deployment

Upload the application files to the repository root or `/docs` directory.

Then configure:

```text
Repository Settings
→ Pages
→ Source: GitHub Actions
```

or:

```text
Repository Settings
→ Pages
→ Deploy from a branch
→ Branch: main
→ Folder: /docs
```

---

## Tutorial Drawings

The project includes a full A3 landscape tutorial drawing manual.

The drawing set covers:

* General arrangement
* Half-wing planform
* Dihedral and washout
* Root, midspan, and tip sections
* Structural architecture
* Rib profiles
* Main and rear spars
* Joiner and rear pin
* Aileron and hinges
* Servo installation
* Wingtip assembly
* Skin installation
* Adhesive sequence
* Manufacturing plan
* SOLIDWORKS modelling workflow
* Simulation setup
* Proof-load test fixture
* Final inspection checklist

Suggested file:

```text
OpenWing-UAV-Full-Tutorial-Drawings.pdf
```

---

## Repository Structure

```text
OpenWing-UAV/
├── .github/
│   ├── workflows/
│   ├── ISSUE_TEMPLATE/
│   └── PULL_REQUEST_TEMPLATE.md
│
├── cad/
│   ├── native-solidworks/
│   │   ├── parts/
│   │   ├── assemblies/
│   │   └── drawings/
│   ├── neutral/
│   │   ├── step/
│   │   ├── stl/
│   │   └── 3mf/
│   └── dxf/
│
├── cam/
│   ├── cnc/
│   ├── additive/
│   ├── fixtures/
│   └── setup-sheets/
│
├── simulation/
│   ├── openvsp/
│   ├── vspaero/
│   ├── xfoil/
│   ├── solidworks-fea/
│   ├── neutral-fea/
│   └── load-cases/
│
├── optimisation/
│   ├── design-variables/
│   ├── candidates/
│   ├── results/
│   └── scripts/
│
├── prototype/
│   ├── material-coupons/
│   ├── subcomponent-tests/
│   ├── proof-tests/
│   ├── ultimate-tests/
│   ├── modal-tests/
│   └── correlation/
│
├── data/
│   ├── templates/
│   └── results/
│
├── drawings/
│   ├── tutorial/
│   ├── manufacturing/
│   └── inspection/
│
├── docs/
│   ├── index.html
│   ├── assets/
│   └── downloads/
│
├── scripts/
│   ├── validation/
│   ├── geometry/
│   ├── simulation/
│   ├── optimisation/
│   └── release/
│
├── release/
├── media/
├── schemas/
├── README.md
├── ROADMAP.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── CITATION.cff
├── SECURITY.md
└── LICENSE
```

---

## Available File Formats

The project may contain or generate:

### CAD and Manufacturing

```text
.SLDPRT
.SLDASM
.SLDDRW
.STEP
.STP
.STL
.3MF
.DXF
.SVG
.PDF
```

### Aerodynamic and Simulation

```text
.vsp3
.vspscript
.inp
.vtk
.csv
.json
.txt
```

### Automation and Web

```text
.py
.js
.html
.css
.yml
.yaml
.bat
.md
```

### Important Format Note

STEP, STL, and 3MF files contain transferable geometry but do not preserve original SOLIDWORKS parametric feature history.

Native SOLIDWORKS files should be generated and saved using an installed copy of SOLIDWORKS 2023.

---

## Software Requirements

Depending on the selected workflow:

* SOLIDWORKS 2023
* SOLIDWORKS Simulation
* OpenVSP
* VSPAERO
* XFOIL
* Python 3.11 or newer
* Git
* Git LFS
* Modern web browser
* Optional CNC CAM software
* Optional slicing software for 3D printing

### Python Packages

Most repository-automation scripts use the Python standard library.

The SOLIDWORKS automation workflow may additionally require:

```bash
pip install pywin32
```

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/OWNER/OpenWing-UAV.git
cd OpenWing-UAV
```

Replace `OWNER` with the GitHub username or organisation name.

### 2. Install Git LFS

```bash
git lfs install
git lfs pull
```

### 3. Validate the Repository

```bash
python scripts/validate_repository.py
```

### 4. Generate Dashboard Data

```bash
python scripts/generate_dashboard_data.py
```

### 5. Generate the Release Manifest

```bash
python scripts/build_release_manifest.py
```

### 6. Run All Automation

```bash
make all
```

---

## Running the GitHub Pages App

The application does not require a JavaScript build system.

### Local Use

Open:

```text
index.html
```

in a modern browser.

For browsers that restrict local file loading, run a local HTTP server:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

### GitHub Pages

Push the website to GitHub and enable Pages from the repository settings.

---

## SOLIDWORKS 2023 Workflow

The repository includes a Windows automation package for importing STEP files into SOLIDWORKS 2023.

The workflow can:

1. Open STEP models.
2. Run import diagnostics.
3. Save imported parts as `.SLDPRT`.
4. Build assemblies as `.SLDASM`.
5. Create third-angle drawings as `.SLDDRW`.
6. Export drawing PDFs.
7. Produce conversion logs.

Example launcher:

```text
RUN_SOLIDWORKS_2023_CONVERTER.bat
```

The conversion creates genuine SOLIDWORKS files only when executed on a Windows PC with SOLIDWORKS 2023 installed.

Imported STEP files become native imported-body features. They do not automatically recover the original sketches, equations, loft history, mates, or design intent.

---

## OpenVSP Workflow

The OpenVSP workflow includes:

* Python model generator
* AngelScript generator
* Wing planform configuration
* NACA 4412 section definition
* Dihedral and twist
* Native `.vsp3` generation
* STEP, STL, and DXF exports

Example generator files:

```text
generate_openwing_vsp.py
generate_openwing.vspscript
RUN_OPENVSP_GENERATOR.bat
```

---

## Python Automation

The project includes scripts for:

* NACA 4412 profile generation
* Root, midspan, and tip coordinate generation
* Load-band scaling
* Gust-load preparation
* Rotating-excitation mapping
* Candidate ranking
* FEA-to-test error calculation
* CSV schema checking
* Repository validation
* Dashboard-data generation
* Release-manifest generation
* SHA-256 file hashing
* SOLIDWORKS automation
* OpenVSP automation

---

## Validation and Reproducibility

The project uses the following reproducibility principles:

* Every released model receives a revision.
* Baseline inputs are never silently overwritten.
* Raw solver data remain separate from processed results.
* Numerical values include units and source descriptions.
* Failed studies are retained and documented.
* CAD, manufacturing, and analysis files remain revision-aligned.
* Release files receive SHA-256 hashes.
* CSV templates use controlled headers.
* GitHub Actions checks repository structure.
* Generated dashboard files are compared with committed versions.
* Preliminary models are not presented as certification evidence.

### Release Manifest

Run:

```bash
python scripts/build_release_manifest.py
```

This generates:

```text
release/manifest.csv
release/manifest.json
```

---

## Known Limitations

The current project has the following limitations:

1. The wing has not yet completed a full physical proof and ultimate test programme.
2. Material properties require coupon testing using the actual manufacturing process.
3. Reference aerodynamic results are not equivalent to validated viscous CFD or wind-tunnel data.
4. Neutral beam results are simplified and are not final detailed SOLIDWORKS Simulation results.
5. Imported STEP models do not preserve full parametric SOLIDWORKS history.
6. Generic CAM files must not be used without machine-specific verification.
7. Modal analysis alone does not establish flutter safety.
8. Potential-flow analysis does not accurately predict separated stall behaviour.
9. Complete-aircraft stability, propulsion, energy, and flight-control integration remain future work.
10. The design is not certified for flight or commercial operation.

---

## Project Status

| Workstream                            | Status        |
| ------------------------------------- | ------------- |
| Baseline requirements                 | Complete      |
| Parametric airfoil profiles           | Complete      |
| External wing geometry                | Complete      |
| Structural architecture               | Complete      |
| Neutral CAD generation                | Complete      |
| Tutorial drawings                     | Complete      |
| Live 3D web application               | Complete      |
| Aerodynamic workflow                  | Complete      |
| Reference aerodynamic outputs         | Available     |
| Structural simulation workflow        | Complete      |
| Neutral structural outputs            | Available     |
| Optimisation workflow                 | Complete      |
| Prototype-test planning               | Complete      |
| Native SOLIDWORKS conversion workflow | Available     |
| OpenVSP native generation workflow    | Available     |
| Material coupon testing               | Not completed |
| Full detailed FEA validation          | Not completed |
| Physical proof testing                | Not completed |
| Modal test correlation                | Not completed |
| Complete-aircraft integration         | Not completed |
| Flight readiness                      | Not claimed   |

---

## Conclusion

The OpenWing-UAV project demonstrates a complete, traceable, and multidisciplinary workflow for developing a modular uncrewed-aircraft wing from an initial aerodynamic concept to a digitally documented engineering system.

Beginning with the Version 0.1 parametric wing definition, the project progressively integrated airfoil generation, planform geometry, dihedral, washout, structural architecture, control surfaces, modular joiner systems, manufacturing preparation, aerodynamic assessment, structural simulation, optimisation, prototype-test planning, and repository automation through Version 0.9.

The baseline design uses a 1.2 m tapered wing with a NACA 4412 airfoil, 3° dihedral, −2° tip washout, internal spars and ribs, a removable joiner system, and an integrated aileron and servo arrangement. A consistent digital thread connects CAD geometry, manufacturing files, aerodynamic loads, structural load cases, modal and buckling studies, optimisation variables, test procedures, and project documentation.

A major strength of the project is that CAD, simulation, manufacturing, testing, and documentation are treated as connected engineering activities rather than isolated tasks. Aerodynamic loads feed structural studies, optimisation is constrained by strength and manufacturability, and physical tests are designed to correlate and improve the computational models.

The generated neutral CAD files, drawings, scripts, aerodynamic references, structural templates, optimisation tools, prototype-test plans, repository automation, and live 3D application provide a practical foundation for further development.

OpenWing-UAV therefore fulfils its purpose as an open-source aerospace engineering portfolio project. It demonstrates skills in parametric design, aerodynamics, structural mechanics, optimisation, digital manufacturing, experimental planning, software automation, technical documentation, data management, and interactive web development.

The current design should be regarded as a documented engineering prototype rather than a flight-certified aircraft component. Final flight-readiness decisions must follow physical material testing, detailed model validation, complete-aircraft integration, safety assessment, regulatory review, ground testing, and controlled flight testing.

---

## Future Enhancements

### 1. Fully Parametric Native SOLIDWORKS Models

Rebuild all imported neutral geometry as native SOLIDWORKS parts and assemblies using:

* Equation-driven sketches
* Design tables
* Parametric lofts
* Configurations
* Assembly mates
* Automated drawings
* BOM-linked custom properties
* Manufacturing configurations

This would preserve complete design intent and allow automatic resizing.

### 2. Higher-Fidelity Aerodynamics

Add:

* Viscous CFD
* Transition modelling
* Stall progression
* Propeller–wing interaction
* Control-surface gaps
* Ground effect
* Sideslip
* Unsteady gust response
* Wind-tunnel correlation
* Flight-pressure measurements

### 3. Composite Laminate Modelling

Define:

* Ply materials
* Ply orientations
* Stacking sequence
* Fibre volume fraction
* Cure process
* Core material
* Bond-line thickness
* Manufacturing tolerances

Apply composite failure criteria such as:

* Tsai–Wu
* Hashin
* Maximum stress
* Maximum strain
* Interlaminar shear
* Delamination screening

### 4. Detailed Joint and Adhesive Analysis

Improve:

* Joiner-box contact
* Adhesive peel modelling
* Cohesive-zone behaviour
* Pin bearing
* Clearance sensitivity
* Bolt preload
* Friction
* Progressive joint failure
* Root-rib bearing
* Hinge-lug fatigue

### 5. Aeroelasticity and Flutter

Add:

* Static divergence
* Control reversal
* Flutter-speed estimation
* Servo stiffness
* Hinge free play
* Mass balancing
* Gust response
* Motor-order excitation
* Propeller blade-pass excitation
* Aeroelastic model correlation

### 6. Complete-Aircraft Integration

Develop:

* Fuselage
* Tail surfaces
* Landing or launch system
* Propulsion
* Battery system
* Avionics
* Payload
* Cooling
* Wiring
* Maintenance access
* Complete mass properties
* Centre-of-gravity envelope

### 7. Propulsion and Energy Optimisation

Add:

* Motor selection
* Propeller matching
* Electronic speed controller sizing
* Battery sizing
* Endurance analysis
* Climb performance
* Thermal modelling
* Power reserve
* Voltage-drop analysis
* Vibration monitoring

### 8. Multidisciplinary Optimisation

Extend the current optimisation to include:

* Aerodynamic efficiency
* Structural mass
* Endurance
* Cost
* Manufacturing time
* Noise
* Reliability
* Stability
* Repairability

Possible methods include:

* Latin-hypercube sampling
* Genetic algorithms
* Bayesian optimisation
* Surrogate modelling
* Monte Carlo uncertainty analysis

### 9. Manufacturing Automation

Add:

* Validated machine-specific CNC files
* Post-processors
* Tool libraries
* Cutting layouts
* Material nesting
* Drill jigs
* Assembly fixtures
* Composite moulds
* Print profiles
* Inspection gauges
* Digital work instructions

### 10. Physical Prototype Testing

Complete:

* Material coupons
* Main-spar bending test
* Root-joiner test
* Hinge and servo tests
* Positive proof load
* Negative proof load
* Positive ultimate test
* Negative ultimate test
* Modal impact test
* FEA-to-test correlation

### 11. Hardware-in-the-Loop Testing

Integrate:

* Autopilot hardware
* Servos
* Sensors
* Communication links
* Telemetry
* Actuator limits
* Navigation software
* Failure handling
* Software-in-the-loop simulation
* Hardware-in-the-loop simulation

### 12. Flight-Test Programme

Create a controlled sequence for:

* Ground inspection
* Control checks
* Propulsion tests
* Restrained tests
* Initial low-risk flight
* Envelope expansion
* Endurance flights
* Gust testing
* Emergency-procedure validation
* Post-flight structural inspection

### 13. Safety and Regulatory Development

Add:

* Hazard analysis
* Failure-mode-and-effects analysis
* Operational risk assessment
* Maintenance intervals
* Inspection procedures
* Component life limits
* Lost-link logic
* Geofencing
* Emergency recovery
* Applicable regulatory requirements

### 14. Digital Twin

Connect real telemetry to the 3D model:

* Strain
* Vibration
* Temperature
* Battery condition
* Servo position
* Flight loads
* Fatigue accumulation
* Maintenance warnings
* Historical mission replay

### 15. Enhanced Web Application

Extend the GitHub Pages app with:

* glTF loading
* STEP-derived visual assets
* Exploded assemblies
* Section-cut tools
* Measurement tools
* Result contours
* Interactive plots
* Version comparisons
* Offline progressive-web-app installation
* Accessibility improvements

### 16. Automated Engineering Pipeline

Develop one controlled configuration file that can automatically generate:

* Airfoil profiles
* CAD parameters
* OpenVSP models
* Aerodynamic loads
* FEA inputs
* Optimisation scenarios
* Plots
* Drawings
* Documentation
* Website data
* Release manifests

### 17. Open Community Configurations

Allow contributors to submit:

* Alternative airfoils
* Different spans
* Different materials
* Alternative joiners
* Different propulsion systems
* New manufacturing processes
* Experimental results
* Additional analysis tools

All contributions should preserve common units, metadata, naming, licensing, and validation rules.

### 18. Version 1.0 Reproducible Release

Version 1.0 should contain:

* Final selected native CAD
* Released neutral CAD
* Manufacturing drawings
* Completed aerodynamic results
* Converged structural studies
* Material-property sources
* Prototype-test results
* Correlated FEA model
* Documented limitations
* Tagged release package
* Verified SHA-256 manifest

### 19. Complete Open UAV Platform

The long-term goal is to expand OpenWing-UAV into a complete modular uncrewed-aircraft development platform supporting:

* Aerospace education
* Environmental monitoring
* Mapping
* Research payloads
* Autonomous navigation
* Structural-health monitoring
* Comparative configuration studies
* Open and reproducible flight-test research

---

## Roadmap

```text
Version 1.0
Reproducible wing engineering release

Version 2.0
Complete aircraft integration

Version 3.0
Flight-test and telemetry digital thread
```

See [ROADMAP.md](ROADMAP.md) for the detailed roadmap.

---

## Safety Notice

This repository contains engineering geometry, structural calculations, test procedures, and manufacturing references.

Before manufacturing or testing:

* Verify all dimensions.
* Confirm material properties.
* Review machine settings.
* Simulate CAM outputs.
* Inspect imported CAD.
* Recalculate loads.
* Use calibrated instrumentation.
* Establish exclusion zones.
* Use remote loading for structural tests.
* Follow applicable UAV regulations.
* Obtain qualified engineering review where required.

Do not use generic NC or G-code directly on a machine without reviewing:

* Controller compatibility
* Units
* Coordinate system
* Tool length
* Feed rate
* Spindle speed
* Workholding
* Clearance
* Stock dimensions
* Emergency-stop procedure

This project does not provide certification, airworthiness approval, or permission to operate an aircraft.

---

## Contributing

Contributions are welcome in areas such as:

* CAD improvements
* Aerodynamics
* Structural analysis
* Materials
* Manufacturing
* Testing
* Automation
* Documentation
* Web development
* Data visualisation

Before submitting a pull request, include:

1. The problem or requirement.
2. The affected revision.
3. The changed assumptions.
4. Validation evidence.
5. Regenerated derived files.
6. Known limitations.

See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Citation

Citation metadata is provided in:

```text
CITATION.cff
```

Suggested citation:

```text
Samuelson G. OpenWing-UAV: An Open Parametric CAD, CAM,
Aerodynamic, Structural Validation, Optimisation, and Prototype
Testing Framework for a Modular Uncrewed-Aircraft Wing. 2026.
```

---

## License

The repository scaffold, scripts, and documentation are released under the MIT License unless otherwise stated.

See [LICENSE](https://github.com/Samuelson777/OpenWing-UAV/blob/main/LICENSE).

Before publishing third-party datasets or engineering files, confirm redistribution rights for:

* Airfoil data
* Material databases
* Standards
* CAD libraries
* Software-generated assets
* Test data
* Manufacturer specifications

---

## Author

**Samuelson G**

OpenWing-UAV is developed as an open-source aerospace engineering, research, automation, and portfolio project.

---

## Acknowledgement

This project uses concepts and workflows associated with:

* Parametric CAD
* OpenVSP
* VSPAERO
* XFOIL
* Finite-element analysis
* Composite structures
* Experimental modal analysis
* Multidisciplinary design optimisation
* GitHub Actions
* GitHub Pages
* Open engineering documentation

---

## Final Statement

OpenWing-UAV is not only a wing model. It is a complete engineering-development framework connecting requirements, geometry, analysis, manufacturing, testing, optimisation, documentation, and public communication in one traceable open-source project.
