# LTC3807 Synchronous Buck Converter (5V to 1V, 3A) – Simulation and PCB Design

This repository contains the complete circuit simulation in **LTspice**, schematic capture, 2-layer PCB layout in **KiCad**, as well as full manufacturing files and documentation for a synchronous step-down (buck) power supply based on the **LTC3807EFE** controller.

## Technical Specifications
* **Controller IC:** Analog Devices LTC3807EFE
* **Input Voltage:** 5V DC
* **Output Voltage / Current:** 1V DC / 3A
* **PCB Stackup:** 2-layer PCB (`F.Cu` and `B.Cu`) featuring a solid ground plane (`GND`) on the bottom layer for optimal EMC shielding and low return-path inductance
* **Verification Status:** Passed KiCad Design Rule Check (DRC) with 0 errors and 0 warnings

## Repository Structure and Contents
* **`LTspice/`** – Simulation files (`Buck_converter_5V_til_1V_3A.asc` and `.plt` plot settings) used to verify output voltage regulation and ripple prior to PCB layout.
* **`Levering/`** – Complete manufacturing and documentation deliverables:
  * **`1_Kortet_i_3D.pdf`** – 3D renders of the top and bottom sides of the finished PCB.
  * **`2_Samledokument.pdf`** – Combined documentation package including the schematic, 2D PCB layout, DRC report (0 errors and 0 warnings), and Bill of Materials.
  * **`Gerber/`** – Manufacturing Gerber files in Protel format (`.gtl`, `.gbl`, `.gko`, `.gts`, `.gbs`, `.gto`, `.gbo`).
  * **`NC Drill/`** – Excellon drill file (`.TXT`).
  * **`BOM/`** – Complete Bill of Materials in Excel (`.xlsx`) calculated for 4 boards with DigiKey part numbers.
* **KiCad Project Files (`TLC3807_prosjekt.*`)** – Complete source files for the schematic (`.kicad_sch`), PCB layout (`.kicad_pcb`), and project configuration (`.kicad_pro`).

---
*Designed and documented by Bjørnar Mogård.*
