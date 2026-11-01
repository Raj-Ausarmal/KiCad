###### \# LED-PCB

###### 

###### A simple LED circuit designed and laid out as a PCB using KiCad 10.0.6.

###### 

###### \## Project Overview

###### 

###### This project documents the design of a single-LED PCB, from schematic creation to PCB layout and fabrication-file generation. It was created as a practice project to learn the basic PCB design workflow.

###### 

###### \## Circuit

###### 

###### The circuit uses a current-limiting resistor in series with an LED. Power is applied through the board’s input connections.

###### 

###### \## Design Workflow

###### 

###### 1\. Created the circuit schematic in KiCad.

###### 2\. Transferred the circuit to the PCB editor.

###### 3\. Placed components and routed the board.

###### 4\. Checked the design using KiCad’s Design Rules Checker (DRC).

###### 5\. Generated Gerber and drill files for fabrication.

###### 

###### \## Design Validation

###### 

###### The PCB was checked with KiCad’s DRC and reviewed in the 3D Viewer.

###### 

###### \## Repository Structure

###### 

###### LED-PCB/

###### ├── gerbers/

###### │   ├── F\_Cu.gbr

###### │   ├── B\_Cu.gbr

###### │   ├── F\_Mask.gbr

###### │   ├── B\_Mask.gbr

###### │   ├── F\_Silkscreen.gbr

###### │   ├── B\_Silkscreen.gbr

###### │   ├── Edge\_Cuts.gbr

###### │   ├── PTH.drl

###### │   ├── NPTH.drl

###### │   └── \*.gbrjob

###### │

###### ├── hardware/

###### │   ├── LED-PCB.kicad\_pcb

###### │   ├── LED-PCB.kicad\_pro

###### │   └── LED-PCB.kicad\_sch

###### │

###### ├── images/

###### │   ├── 3d\_view.png

###### │   ├── pcb\_layout.png

###### │   └── schematic.png

###### │

###### └── README.md

