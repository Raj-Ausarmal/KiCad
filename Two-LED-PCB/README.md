# Two-LED-PCB

A simple battery-powered LED PCB designed using KiCad.

This is one of my beginner PCB design projects where I practiced the PCB workflow, from creating the schematic to designing the PCB layout, routing the connections, checking the board with DRC, and generating Gerber files.

## Overview

The circuit is a simple series circuit:

**Battery + → Resistor → LED → Battery −**

When power is connected, current flows through the resistor and LED, turning the LED on.

## Circuit Components

| **Reference** | **Component** | **Value / Type** |
| ------------- | ------------- | ---------------- |
| J1 | 2-Pin Connector | Power Input |
| R1 | Resistor | Current-limiting resistor |
| D1 | LED | Through-hole |

## PCB Design

The PCB was designed using **KiCad 10.0.6**.

- PCB type: Through-hole components
- Routing layer: Front Copper (F.Cu)

## PCB Validation

After completing the PCB routing, I ran KiCad's Design Rules Checker (DRC).

- Unrouted connections: **0**
- DRC violations: **0**

The PCB was also checked using KiCad's 3D Viewer.

## Project Structure

Two-LED-PCB/
│
├── gerbers/
│   ├── Gerber fabrication files
│   ├── Drill files
│   └── Gerber job file
│
├── hardware/
│   ├── Two-LED-PCB.kicad_pcb
│   ├── Two-LED-PCB.kicad_pro
│   └── Two-LED-PCB.kicad_sch
│
├── images/
│   ├── 3d_view.png
│   ├── pcb_layout.png
│   └── schematic.png
│
└── README.md