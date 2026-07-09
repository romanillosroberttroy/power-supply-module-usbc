# Power Supply Module — USB-C Dual Output (5V / 3.3V)

## Overview
A compact, clean power supply board designed for IoT and embedded system projects.
Takes USB-C input and outputs regulated 5V and 3.3V rails with proper decoupling,
protection, and indicator LEDs.

## Features
- USB-C input connector
- 5V output via USB pass-through
- 3.3V output via AMS1117-3.3 LDO regulator
- Polarity protection MOSFET
- Bulk and decoupling capacitors on all rails
- LED power indicators for both output rails
- Test points on all voltage rails
- Mounting holes for enclosure integration

## Schematic
![Schematic](images/schematic.png)

## PCB Layout
![PCB Front](images/pcb-front.png)
![PCB Back](images/pcb-back.png)

## 3D Render
![3D View](images/3d-render.png)

## Design Notes
- AMS1117-3.3 requires a minimum 10uF output capacitor for stability
- 100nF decoupling capacitors placed within 1mm of each power pin
- Polarity protection using P-channel MOSFET to prevent reverse voltage damage
- Board designed for JLCPCB 2-layer standard stackup

## Fabrication
- Designed for JLCPCB 2-layer PCB
- Minimum trace width: 0.2mm
- Minimum clearance: 0.2mm
- Board dimensions: 40mm x 30mm
- Gerber files available in /gerbers folder

## Bill of Materials
See /bom/bom.csv for complete component list with LCSC part numbers.
