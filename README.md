# USB Hub PCB Project

Short description
-----------------

This repository contains the design files and results for a USB hub PCB project. It includes Altium Designer schematics and PCB documents, electromagnetic / signal integrity results, and screenshots.

Repository structure
--------------------

- AEDT/ — HFSS/Ansys Electronics Desktop screenshots and exports
- ALTIUM DESIGNS/ — Altium project files
  - PCB_DESIGN/
    - usb_hub.PcbDoc
    - USB.PcbDoc
  - SCHEMATIC/
    - usb_hub.SchDoc
- RESULTS/ — export and manufacturing output (ODB, layers, netlists, screenshots)
- ANSYS SIWAVE/ — SIwave setup and screenshots

Key files
---------

- Altium PCB: [ALTIUM DESIGNS/PCB_DESIGN/usb_hub.PcbDoc](ALTIUM%20DESIGNS/PCB_DESIGN/usb_hub.PcbDoc)
- Altium Schematic: [ALTIUM DESIGNS/SCHEMATIC/usb_hub.SchDoc](ALTIUM%20DESIGNS/SCHEMATIC/usb_hub.SchDoc)
- Manufacturing outputs: RESULTS/odb/

Opening and viewing
--------------------

- To edit or view the PCB and schematic, open the .PcbDoc and .SchDoc files in Altium Designer.
- Manufacturing outputs in RESULTS/odb/ can be inspected with CAM/ODB viewers or imported into CAM software.
- Ansys/Siwave exports and screenshots are stored under ANYSYS SIWAVE/ and AEDT/ respectively.

Notes
-----

- Keep Altium project backups before performing automated conversions or panelization.
- This repository is organized for offline CAD and simulation workflows — no build scripts are included.

Contact
-------

For questions about the design files, contact the project owner.
