# PCB-LED-PushButton

A simple LED and push-button PCB designed using KiCad.

This is one of my beginner PCB design projects where I practiced the complete PCB workflow, from creating the schematic to designing the PCB layout, routing the connections, checking the board with DRC, and generating Gerber files.

## Overview

The circuit is a simple series circuit:

**Battery + → Push Button → 330Ω Resistor → LED → Battery −**

When the push button is pressed, current flows through the resistor and LED, turning the LED on.

## Circuit Components

| Reference | Component | Value / Type |
|---|---|---|
| J1 | 2-Pin Connector | Power Input |
| SW1 | Push Button | THT |
| R1 | Resistor | 330Ω |
| D1 | LED | 5mm |

## PCB Design

The PCB was designed using **KiCad 10.0.6**.

### Board Size

- Length: 60 mm
- Width: 21.5 mm
- PCB type: Through-hole components
- Routing layer: Front Copper (F.Cu)

The components are arranged in a simple left-to-right layout:

**J1 → SW1 → R1 → D1**

## PCB Validation

After completing the PCB routing, I ran KiCad's Design Rules Checker (DRC).

Final result:

- Unrouted connections: **0**
- DRC violations: **0**
- Unconnected items: **0**
- Errors: **0**
- Warnings: **0**

The PCB was also checked using KiCad's 3D Viewer.

## Project Structure

```text
PCB-LED-PushButton/
│
├── docs/
│
├── gerbers/
│   ├── F_Cu.gbr
│   ├── B_Cu.gbr
│   ├── F_Mask.gbr
│   ├── B_Mask.gbr
│   ├── F_Silkscreen.gbr
│   ├── B_Silkscreen.gbr
│   ├── Edge_Cuts.gbr
│   ├── PTH.drl
│   ├── NPTH.drl
│   └── *.gbrjob
│
├── hardware/
│   ├── PCB-LED-PushButton.kicad_pcb
│   ├── PCB-LED-PushButton.kicad_pro
│   └── PCB-LED-PushButton.kicad_sch
│
├── images/
│   ├── 3d_view.png
│   ├── pcb_layout.png
│   └── schematic.png
│
└── README.md