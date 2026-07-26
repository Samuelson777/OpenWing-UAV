# OpenWing-UAV Complete Engineering Package

This package combines all previously created project files with the newly generated engineering deliverables.

## Newly generated

- 32 watertight part geometries
- 35 AP203 faceted STEP files
- 35 STL files
- 35 3MF files
- 16 DXF drawings and SVG previews
- 13 generic, unverified NC files
- Right-wing and full-wing geometry assemblies
- Completed lifting-line aerodynamic result CSVs
- Completed equivalent beam-FEA static and modal results
- Neutral CalculiX/Abaqus-style input deck and VTK result
- OpenVSP scripts that generate the native `.vsp3` model and OpenVSP exports
- SOLIDWORKS COM automation that generates `.SLDPRT`, `.SLDASM`, and `.SLDDRW` files when run on Windows with SOLIDWORKS installed

## Remaining application-dependent outputs

Native SOLIDWORKS binaries and the native OpenVSP `.vsp3` file cannot be written without those installed applications. The package includes executable generator scripts for them rather than fake files. Native SOLIDWORKS Simulation databases and machine-approved G-code also require the licensed solver and actual machine/postprocessor.

Start with:

`02_GENERATED_ENGINEERING_FILES/08_DOCUMENTATION/README_FIRST.md`
