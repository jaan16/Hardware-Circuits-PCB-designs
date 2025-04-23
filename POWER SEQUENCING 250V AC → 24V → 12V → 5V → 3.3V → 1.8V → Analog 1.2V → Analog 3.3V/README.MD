
# Power System Design for Power Sequencing

## Overview

This repository contains the design files for a power system that provides multiple voltage domains with a specific power-up sequence. The system takes a 250V AC input and regulates it down to the following DC voltage levels in the specified order:

**Power Sequence:** 250V AC → 24V → 12V → 5V → 3.3V → 1.8V → Analog 1.2V → Analog 3.3V

This power sequencing is crucial for the proper operation of the downstream loads and to prevent potential damage or instability.

## Load Requirements

The power system is designed to supply the following loads:

* **1.8V:** 100mA
* **Analog 1.2V:** 150mA
* **Analog 3.3V:** 100mA
* **3.3V:** 10mA
* **5V:** 5mA
* **12V:** 300mA

## Contents

This repository includes the following files:

* **Schematic:** (Name of your schematic file, e.g., `Power_System_Schematic.pdf`, `Power_System_Schematic.sch`) - Contains the detailed circuit diagram of the power system.
* **Bill of Materials (BOM):** (Name of your BOM file, e.g., `Power_System_BOM.xlsx`, `Power_System_BOM.csv`) - Lists all the components required for the power system, including part numbers, manufacturers, and quantities.
* **Datasheets:** (Directory or individual files containing relevant component datasheets) - Includes the datasheets of key components used in the design, which were referred to during the design process. Please ensure the filenames are descriptive (e.g., `LMR33630_Datasheet.pdf`, `TPS7A4700_Datasheet.pdf`).

## Design Considerations

The design incorporates specific considerations for the power sequencing requirement. This likely involves the use of supervisory circuits, enable pins, or other techniques to ensure the voltage rails power up in the defined order. The schematic and BOM will provide details on the implementation of this sequencing.
