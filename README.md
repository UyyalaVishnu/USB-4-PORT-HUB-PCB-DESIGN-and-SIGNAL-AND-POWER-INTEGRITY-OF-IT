# USB Hub PCB Project

Project overview
----------------

This repository contains the design source, simulation exports, and manufacturing outputs for a 4-port USB hub PCB. The files are maintained for design review, fabrication, and signal/power integrity analysis. Primary CAD source files were created in Altium Designer; simulation exports were generated using Ansys (AEDT / SIwave).

Features
--------

- Full Altium schematic and PCB source files for the USB hub design
- Exported manufacturing data (ODB++, Gerber-like layer exports, netlists)
- Simulation inputs and screenshots for HFSS / SIwave workflows

Repository layout
-----------------

- AEDT/ — HFSS/Ansys Electronics Desktop screenshots and exports
- ALTIUM DESIGNS/
  - PCB_DESIGN/
    - usb_hub.PcbDoc
    - USB.PcbDoc
  - SCHEMATIC/
    - usb_hub.SchDoc
- RESULTS/
  - odb/ — ODB++ exports and CAM-ready files
    - layers/ — layer-specific feature exports
    - netlists/ — exported netlists and CADNET files
  - SCREENSHOTS/ — manufacturing and review images
- ANSYS SIWAVE/ — SIwave projects and exported datasets

Key files (quick links)
----------------------

- Altium PCB: [ALTIUM DESIGNS/PCB_DESIGN/usb_hub.PcbDoc](ALTIUM%20DESIGNS/PCB_DESIGN/usb_hub.PcbDoc)
- Altium Schematic: [ALTIUM DESIGNS/SCHEMATIC/usb_hub.SchDoc](ALTIUM%20DESIGNS/SCHEMATIC/usb_hub.SchDoc)
- Manufacturing outputs folder: [RESULTS/odb](RESULTS/odb/)

Prerequisites
-------------

- Altium Designer (recommended) to open and edit `.SchDoc` and `.PcbDoc` files.
- CAM/ODB viewer (for ODB++ or Gerber inspection) — e.g., GerbView, CAM350, or online viewers.
- Ansys AEDT / SIwave for simulation project files and advanced analysis.

How to open and review
----------------------

1. Open the Altium project in Altium Designer by opening the schematic or PCB document in `ALTIUM DESIGNS/`.
2. Use Altium's CAM outputs to generate Gerbers/ODB for the manufacturer. Verify layer stack and drill tables before release.
3. Inspect `RESULTS/odb/` with a CAM tool to review fabrication artifacts and exported feature lists.
4. For SI/PI analysis, open the projects under `ANYSYS SIWAVE/` or `AEDT/` in the corresponding Ansys tools.

Export & fabrication notes
--------------------------

- Verify DRL and drill tool settings when producing Gerbers or ODB exports.
- Confirm layer stackup, dielectric thicknesses, and impedance targets before releasing to fabrication.
- Include assembly drawings and pick-and-place files if providing BOM/assembly to the manufacturer.

Simulation and measurement notes
-------------------------------

- SIwave/HFSS exports were used for impedance and crosstalk analysis — see `ANYSYS SIWAVE/` and `AEDT/` for screenshots and exported datasets.
- Keep measurement reference points and connector pin assignments documented when correlating simulation results to measurements.

File naming and versioning
-------------------------

- Source files: keep original Altium filenames intact (e.g., `usb_hub.SchDoc`, `usb_hub.PcbDoc`).
- Exports: include date and tool version in export filenames where possible (e.g., `usb_hub_gerber_2026-07-06.zip`).

Contributing
------------

- For changes to the design files, create a branch, update the Altium source files, and include a short commit message describing the change.
- Do not edit binary `.PcbDoc`/.SchDoc files outside of Altium — use Altium's SVN/Git support or generate clear diffs/exports for review.

License
-------

This repository does not include a license file. Add a `LICENSE` if you intend to allow reuse or contributions.

Contact
-------

If you need additional details or files, open an issue or contact the repository owner.

