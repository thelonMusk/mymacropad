# AatieshPad

AatieshPad is a custom 4-key macropad built as part of Hack Club's Hackpad program. It is based on the reference design from the Hackpad guide, with modifications including an additional key and custom firmware configuration.

The macropad uses a Seeed Studio XIAO RP2040 microcontroller and runs QMK firmware, allowing programmable macros and shortcuts for productivity and everyday use.

## Features

* 4 Mechanical Keys
* Custom PCB designed in KiCad
* Custom 3D-printed case designed in Fusion 360
* USB-C Connectivity
* QMK Firmware
* VIA Compatibility
* Fully Programmable Macros

---

# PCB Design

The PCB was designed in KiCad following the Hackpad guide.

## Schematic

The schematic consists of:

* 1 × Seeed Studio XIAO RP2040
* 4 × Mechanical Switches
* 4 × Diodes
* Ground connections for all switches

Each switch is connected to a dedicated GPIO pin on the XIAO RP2040, allowing each key to be detected independently by QMK firmware.

## PCB Layout

After creating the schematic, the PCB was routed manually in KiCad.

Features include:

* Single-sided routing
* Compact layout
* Through-hole switch mounting
* USB-C access through the XIAO RP2040

The board outline was created using the Edge.Cuts layer before exporting the manufacturing files.

### PCB Render

<img width="1004" height="593" alt="Screenshot_2" src="https://github.com/user-attachments/assets/5b6bfdac-a973-4a44-87d8-d91065b743fc" />

### PCB Screenshot

<img width="263" height="683" alt="Screenshot_15" src="https://github.com/user-attachments/assets/ef3926b8-acef-4343-8bd4-53176b88c819" />

---

# Case Design

The enclosure was designed in Fusion 360.

The design follows a sandwich-style construction similar to the Hackpad reference project.

## Components

* Bottom case
* Switch plate
* USB cutout for the XIAO RP2040
* Mounting holes for assembly

The dimensions were based on the final PCB size with additional clearance to account for 3D-printing tolerances.

### Case Render
<img width="1072" height="709" alt="Screenshot_1" src="https://github.com/user-attachments/assets/bc30f4b6-63b2-4b26-81b1-3455193ae108" />


---

# Firmware

The firmware is based on QMK.

Current key functions are:

| Key   | Function |
| ----- | -------- |
| Key 1 | Copy     |
| Key 2 | Paste    |
| Key 3 | Shift Lock |
| Key 4 | customised command    |

The key assignments can be changed through VIA without reflashing the firmware.

## VIA Support

VIA allows the macropad to be reconfigured in real time.

Possible uses include:

* Application shortcuts
* Media controls
* Discord shortcuts
* Coding macros
* Productivity workflows

---

# Bill of Materials

| Quantity | Component                    |
| -------- | ---------------------------- |
| 1        | Seeed Studio XIAO RP2040     |
| 4        | Cherry MX Switches           |
| 4        | Keycaps                      |
| 4        | 1N4148 Diodes                |
| 1        | Custom PCB                   |
| 1        | 3D Printed Case              |
| Various  | Screws and mounting hardware |

---

# What I Learned

This project gave me experience with:

* PCB schematic design in KiCad
* PCB routing
* PCB manufacturing workflows
* CAD design in Fusion 360
* QMK firmware configuration
* VIA integration
* Hardware assembly and soldering

Although the project followed the Hackpad guide as a starting point, building the macropad provided hands-on experience with the complete process of designing, manufacturing, assembling, and programming a custom input device.

---

# Acknowledgements

Special thanks to Hack Club and the Hackpad guide for providing the resources and documentation needed to build this project.

Hackpad is a great introduction to PCB design, firmware development, CAD modelling, and electronics manufacturing.
