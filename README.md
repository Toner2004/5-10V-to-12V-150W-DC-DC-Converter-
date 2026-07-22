
# 5-10V-to-12V-150W-DC-DC-Converter
150W Synchronous Boost Converter (5–10V to 12V) Based on TI LM5123-Q1

A high-power synchronous boost converter designed to convert a 5V–10V input source into a regulated 12V output at up to 150W using the Texas Instruments LM5123-Q1 controller. Its other purpose is to use untested components like automotive connectors for other projects problems with these is unknown footprints.

This project was developed as a complete power electronics design cycle including:

- Schematic capture
- Component selection
- Power stage design
- Compensation design
- PCB layout
- Manufacturing preparation
- Hardware validation

## Specifications

| Parameter | Value |
|------------|------------|
| Controller | TI LM5123-Q1 |
| Topology | Synchronous Boost |
| Input Voltage | 5V – 10V |
| Output Voltage | 12V |
| Output Power | Up to 150W |
| Switching Frequency | ~434 kHz |
| PCB Stackup | 4 Layer |
| Copper Weight | 1 oz |
| Current Sensing | 1.5 mΩ Metal Element Shunt |
| CAD Tool | Altium Designer |
| Manufacturer | JLCPCB |

---

## Key Design Features

### High Current Input Stage

The converter is capable of handling over 30A input current at low input voltages. Large copper pours, multiple stitching vias, and dedicated power routing were implemented to minimize losses and temperature rise.

### 4-Layer PCB

The board utilizes:

- Top Layer: Power Components and Routing
- Layer 1: Solid Ground Plane
- Layer 2: Signal Routing
- Bottom Layer: Additional Signal Routing

This stackup was more forgiving with this size footprint but it also reduces impedance, provides thermal spreading, and improves EMI performance. 

### Low Resistance Current Sensing

A 1.5 mΩ current sense resistor is used to provide accurate current measurement and over-current protection while minimizing power dissipation.

### Thermal Management

Design techniques used include:

- Large copper pours
- Thermal via stitching
- Ground plane heat spreading
- Low RDS(on) MOSFET selection

---

## Design Workflow

1. TI Power Designer used for initial calculations
2. Schematic development in Altium Designer
3. Component selection from DigiKey and Mouser
4. PCB layout optimization
5. DRC verification
6. Gerber and NC drill generation
7. Manufacturing through JLCPCB
   - Redesigns based of manufacturer CAM design faults

---
<img width="791" height="379" alt="Screenshot 2026-07-22 031527" src="https://github.com/user-attachments/assets/20347400-2423-47de-b69d-11e11f9938da" />


<img width="838" height="424" alt="Screenshot 2026-07-22 031459" src="https://github.com/user-attachments/assets/596781e8-fb27-4618-b1f3-66ea0c7a7a70" />

## Repository Contents
